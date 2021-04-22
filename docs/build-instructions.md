## Build Instructions

* Start by going to [Dungeon Run Github](https://github.com/dungeon-run) to view both the service
and client sides of the application. When you select either repository, you will need to select the 
  green code button to then copy the SSH to import into your IDE of choice to import to your own 
  computer.
  
* You must create a project on Google Cloud Console, and create the Android Oauth 2.0 in your project. 
  When you do that, it will ask for an SHA-1 certificate which you must generate from your cloned project in the IDEA.
  This will also allow the client to gain the BearerToken to communicate effectivly with the service
  side of the application.
  
* You will need to create a properties file for the client side and input the client id gained
from the Google cloud console, you will need to input "content_format = %s/content" in another line
  and also the base_url which is the ip address of your emulator device, or physical device if using
  one.
  
* In the Google cloud console you will also need to create the client ID with the Web Service option and
ensure the information is put into the service side of the YML application to run effectively.
  
* Once you have gotten the OAuth keys set up for use on the server and client side of the application,
you will need to first start the server side and ensure the database is generated. Once this is done, 
  you may now start the client side of the application. You will be able to generate your first maze
  by clicking the new button at the top right hand corner of the screen, and start playing.

  
