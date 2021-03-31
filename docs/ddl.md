---
title: Data Definition Language
description: Formatted DDL for Entities Tables and Indexes
menu: ddl
order: 60
---

## Data Definition Language(DDL)

```sql
create table level
(
level_id   CHAR(16) FOR BIT DATA not null,
completed  boolean               not null,
difficulty integer               not null,
end_time   timestamp             not null,
start_time timestamp             not null,
time_given integer               not null,
user_id    CHAR(16) FOR BIT DATA not null,
primary key (level_id)
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
create index IDXop0jc3e424f5dq9xfvgb8sgh1 on level (difficulty, end_time);
create index IDXakmwux4w2swsj69pg3ignha1v on user_profile (created);
create index IDX7amnj5kvh6ct9ihfmqctn97s1 on user_profile (connected);
alter table user_profile
add constraint UK_6f815wi5o4jq8p1q1w63o4mhd unique (oauth_key);
alter table level
add constraint FKjlonrfiin8xslrixn7bmh62gh foreign key (user_id) references user_profile;
```

[![DataDefinitionLanguage](sql/ddl.sql)](sql/ddl.sql)