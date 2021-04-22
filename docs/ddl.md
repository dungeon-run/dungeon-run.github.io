---
title: Data Definition Language
description: Formatted DDL for Entities Tables and Indexes
menu: ddl
order: 60
---

## Data Definition Language(DDL)

```sql
create table attempt
(
    attempt_id   CHAR(16) FOR BIT DATA not null,
    completed    boolean               not null,
    difficulty   integer               not null,
    end_time     timestamp,
    start_time   timestamp             not null,
    time_elapsed bigint                not null,
    time_given   integer               not null,
    user_id      CHAR(16) FOR BIT DATA not null,
    primary key (attempt_id)
);
create table user_profile
(
    user_id   CHAR(16) FOR BIT DATA not null,
    connected timestamp             not null,
    created   timestamp             not null,
    name      varchar(255)          not null,
    oauth_key varchar(255)          not null,
    primary key (user_id)
);
create index IDXiwlmaks3jr7ramydrtc2jxrpg on attempt (difficulty, end_time);
create index IDXakmwux4w2swsj69pg3ignha1v on user_profile (created);
create index IDX7amnj5kvh6ct9ihfmqctn97s1 on user_profile (connected);
alter table user_profile
    add constraint UK_6f815wi5o4jq8p1q1w63o4mhd unique (oauth_key);
alter table attempt
    add constraint FK1051l8tfjbooon82sq66v44tv foreign key (user_id) references user_profile;
```

[DataDefinitionLanguage](sql/ddl.sql)