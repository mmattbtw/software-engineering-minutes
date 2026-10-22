---
{"dg-publish":true,"permalink":"/software-engineering/minutes/","tags":["gardenEntry"],"dg-note-properties":{}}
---


# 10/06/2026
Members Present: Matt, Jack, Hamza, Jesse, Zheer
- Discussed use cases document
- Demoing the Disquisition desktop app with voice
# 10/08/2026
Members Present: Matt, Jack, Jesse, Hamza, Joseph
- Discuss use case document some more
- Bought disquisition.app domain
- Tested screen sharing
# 10/15/2026
Members Present: Matt, Jesse, Jack, Zheer, Hamza
- Work on Use Cases document
- Discussed new stuff like Desktop Notifications and UI Sounds
# 10/20/2026
Members Present: Jack, Matt, Zheer, Jesse
- Discussed new Inter font PR ([PR 67](https://github.com/mmattbtw/disquisition/pull/67))
- Discussed Jack's interface sounds
- Discussed Jack's new App Icons
- Discussed the Server ("Guilds") architecture 
talking about right now. I was thinking about your client: what's hosting the server? You click Create Server and then you're the host. When you give out your invite link, it tells the other person what your IP is, what your invite token is, and what server it is. It's three things in one string.

Most of the time the IP address will just be the relay you're connected to. Pretty much it'll be like a TCP message where it's like, "Hey I'm trying to discover this server," and then they're like, "Okay here is that server." It sends you all the metadata for the server name, the image, who's in it, and that's it pretty much.

The client that's hosting the server sends that data directly to the other person. What if that person goes offline? I think the easiest way to handle that is just whoever's online, or the server just becomes unavailable. That could be an option I guess: migrate host. Could do host migration.

The only problem is what if everybody's offline? You just create a new server or does your client just keep retrying to connect to that server until the other person comes online? Yeah something like that. 

# 10/22/2026
Members Present: Matt, Jesse, Cameron, Hamza, Zheer
- Discussed server/communities architecture: https://www.tldraw.com/f/QburcEqnNyXhKIR1YFsx3?d=v-2262.-1241.4694.3138.page