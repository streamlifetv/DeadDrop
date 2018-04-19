Platform
========

To be a DeadDrop server host requires a Linux, Mac, or Windows machine.

To be a DeadDrop client requires a Tor Browser on any OS.


Install
=======

Install Tor and open Tor Browser Bundle (or the tor client daemon)

Activate your favorite virtualenv e.g..

`$ sudo apt-get install python-virtualenv`

`$ virtualenv dropenv`

`$ source dropenv/bin/activate`

`$ git clone git+https://github.com/acaceres2176/DeadDrop.git`

That's it!

How it works
============

DeadDrop is a disposable mini-chat server that can be used to chat safely and anonymously through Tor. It is
very similar to DropChat, but with a better user experience (no more page reloading at all times here). One
person is the host of the chat server (don't worry being a host only requires one command - no messing with
complex config files) and the others are the clients using only a Tor Browser. The host starts the server 
and shares a URL with the clients. They can then chat with each other safely and anonymously. Once you're 
done sharing the info you want, simply kill the server. No information is stored on disk. There is a RAM
clear script that you can run (if you're on Linux, or possibly Mac) that will clear your RAM for further
safety of your information.

JAVASCRIPT MUST BE ENABLED TO USE DEADDROP. Sorry for shouting, but it is an important difference from our
prior project, dropchat and may cause confusion. This was a hard decision, if you want to complain to me
please do so on Twitter, I'm @_hyp3ri0n. If you really hate JS, use https://github.com/HyperionGray/dropchat
it is a very similar project, but requires no JS. The user experience kind of sucks, but it is also
very safe to use.

Usage
=====

Start Tor or Tor Browser, make sure your Control Port is open and listening on the default port.

`$ python runserver.py`

Share the drop URL with your friends to open in Tor Browser. Chat with them safely and securely!

Features
========

- As chat happens inside the Tor network via ephemeral hidden services, everything is encrypted and attribution of chatters is virtually impossible
- No JS required, use safely with NoScript
- *Nothing* touches disk, everything happens in-memory
- No configuration required
- Low barrier to entry, few dependencies
- No need for a client
- Chats are deleted every 3 minutes
- Randomized usernames - this is for your own safety, so as to decrease chances of username reuse
- New chat service created every time the server is started
- No frills, no fancy CSS, code is easy to follow and review to ensure your safety
- A clear RAM script for use after a DeadDrop session

---

[![define hyperion gray](https://hyperiongray.s3.amazonaws.com/define-hg.svg)](https://hyperiongray.com/?pk_campaign=github&pk_kwd=dropchat "Hyperion Gray")
