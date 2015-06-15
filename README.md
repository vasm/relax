# Relax: Relay XMPP server

# Why?

This software is designed to be a bridge between connection-oriented IM protocols (mainly the awesome XMPP aka Jabber) and REST-oriented platforms, such as iPhone or Android. While XMPP is a cool, extensible and open protocol, it is impossible to connect directly from the devices with energy-efficient task management, as they put the app to the sleep state when it goes to the background, thus breaking their socket connections. So Relax is going to keep the connection up, collect all the incoming notifications and serve them to the user when needed.

Also, it allows for some cool features such as synchronization of message history between your devices (again, impossible with basic Jabber), and keeping attachments on the server for further uses.

## How it works

The relax server stands as a client app which is responsible for connecting to the Jabber server. It also stores all the information (auth, contact list, message history etc.) to make it accessible anytime from any of user's devices.

From the other side, it offers simple, HTTP(S)-based API which allows to do anything that conventional XMPP client would allow. *TODO*: insert wiki link for API.
