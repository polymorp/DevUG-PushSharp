DevUG-PushSharp
===============

This project demonstrates the usage/implementation of the PushSharp .NET SDK for simple and efficient management of multiplatform (IOS, Android and Windows Phone) Push Notification services on the server side. 

This solution is consisted from a couple of separate projects including shared processor libraries; a Web .NET WebAPI    app and a Desktop Windows Forms app used for monitoring and handling push notifications as a "state machine".

The repo is also planned to have 3 (iOS, Android and WP8) client implementations connecting to a implemented PushSharp service server.

ATTENTION: Take care of how much PushNotification objects you will read from the database when processing, in this case there is a thread looping the database for one per one newst push notification. You could also set to read all the notifications instead of one (latest).

Instruction for use
===============
Server: Enter all connection strings to your database where needed, register for push notifications on the service providers: Google, Apple and Microsoft, enter the provided keys to PushNotificationProcessor.cs.

Clients: Enter your 3rd party server endpoints in the PushNotificationHelper.cs

Disclaimer
===============
This demo project was built for a show case on the mscommunity.hr standup/meetup in Zagreb held at 25.11.2014. No coded tests were performed, bugs are possible, please contribute and fork on!

iOS is unfortunately not finished.
