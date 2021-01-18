# **PyBot**

*A fairly simple Discord bot using Python3 and the discord.py (rewrite) library.*

**About this project**

The main goal was to make a simple and modular bot for our servers. 
It is intended to be easy to extend functionality through the addition or removal of cogs without the worry they may depend on each other or provide critical functionality. 
There are by far better (and more complete) bots out there, but this is a fun project to work on regardless. 

**Relevant Info**
- only tested on Windows (10) so far
- there are plans for GNU Linux support (starting with Ubuntu) in the near future
- required libs (packaged with standard python install or otherwise):
   > - discord.py
   > - Fernet
   > - asyncio
   > - aiohttp
   > - ...
   > - {will update with full list soon}

**Current Roadmap ~2020~ 2021**
- minimize external library requirements; ideally only use python standard libraries (not going to happen, but can dream)
- better comments as some places are nearly incomprehensible
- reduce codebase size; many repeated sections can make use of a single semi-modular function instead
- *actually* post the code (after I make it readable for others)
- refactor some portions to make better use of async
- clear out non essential files
- collect code references and help documents into a single document so anyone that comes across this project may find an answer they have been looking for but could never find
- move all non-essential cogs and utility functions into a second repository
   > doing so allows users to customize what functions they want without having to worry about commands/files they do not like or want
- change how log in works for servers during program startup to allow for better recovery when the connection gets interrupted or the program crashes
- update license to an unlicense; see https://unlicense.org
- improve command cache/queue to be more 'robust' as-in not as fragile as it currently is
- MAJOR:
  - convert current data storage method into a single database for ease of use and modularity
    > although the current method is a bit more platform agnostic and easier for an end user/average operator

**Potential Command Ideas**
   > These will be available as optional cogs in a separate repository for use in this bot
- birthday notifications (day + month)
- ? twitch chat integration
- simple giveaways, not likely necessary to support more than a handful at a time
- custom TTS (Text To Speech)
- youtube playlist updater; keeps an updated list of a playlist's contents to allow for better knowledge of what a particular video was if it gets hidden or deleted
- audio player for voice chat (***no*** music provider integration such as youtube, spotify, soundcloud or any others)
- simple games such as Life, Tic Tac Toe, Guess the Number, etc...
- ? passive ATC (Air Traffic Control) integration; the ability to listen to live ATC chatter in a voice channel from a specified region
   > It is possible but will have to consider about how it will be implemented
- modular image manipulation functions
- ? encryption and decryption for messages and files
   > not sure of a use case for a discord bot but will make it standalone as it may be helpful for another project at some point

**Postponed Plans**
- add ability for the optional GUI program (tkinter) to send commands to bot directly
   > probably not helpful in the grand scheme of things
- make 2nd script ensure bot doesn't close and fail to re-open, and add ability to restart at any point
   > could probably just schedule this up in the OS as a repeated task, if the program is not running then start it; would be nice to have this function built-in though

**Notes**
- Scalability is limited
    > It is not intended to run many instances at a time; it probably can deal with at least two at the same time but there could be problems. This can be fixed through stricter adherence to async functions but some are quite difficult to convert to full async.
- Support of this bot for Windows (10) will likely be ending this year as I transition wholly to GNU Linux. I will attempt to keep it at minimum, functional, but may not fix non essential errors. I will still attempt to, but cannot provide any promises.
- I prefer using Python for data analysis and prototyping but a discord bot is a fun challenge. As such, some functionality is quite slow compared to many other languages; keep that in mind when running it. For most tasks it is plenty fast and not too noticable.

**Contact Info:**

*If you have questions or would like to complain about my code, you can communicate with me in these places.*
- *(fastest response)* Discord  |  @sautedmango#4698
- *(overall best)* Email  |  sautedmango@gmail.com
- IRC  | *tbd*

*Last Updated: 18-Jan-21*
