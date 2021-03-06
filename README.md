Connection Planet - SRP Implementation.
=======================================

An implmentation of the SRP (Secure Remote Password) version 6a in the .Net Framework version 4.0.
Created by MusicDemon for Connection Planet.
Purpose; Securing server-client communication without using SSL/TLS etc.
Created after [RFC5054](http://tools.ietf.org/html/rfc5054)

## Story behind
I was wondering how to secure my web-calls from my desktop applications to my website applications. To do this, I wanted to get it working with SRP6a. However, for some reason I seem not to be able to get the to work with [Resource](#Resources)#3, the WSE implementation. So, without a lack of doubt I started this project with hope for a perfect implementation!

## Project setup
The project has been divided by three sub-projects.
- The client library
- The server library (Also referred to as the host.)
- A test console application.

The server library contains functions that are not needed by the client library. However, most of the used functions are used on both libraries, that's why the server library has a reference to the client library.

## Changelog
- 1.4.3.0:
    * Made the libraries .Net 4.5.2.
    * Minor C#.Net 6 syntax changes
    * XML Documentation changes
- 1.1.2.0: Tested several times with same setup. It is working but, in my eye's can use more testing, just to be sure.
- 1.0.0.0: Initial upload. Had issues with formulae like S/x/u.

## Resources
- [RFC5054](http://tools.ietf.org/html/rfc5054)
- [RFC2945](http://tools.ietf.org/html/rfc2945)
- [Channel9](http://channel9.msdn.com/forums/sandbox/secure-remote-password-srp-in-wse)