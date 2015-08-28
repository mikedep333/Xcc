# Xccc
X11 Cached, Compressed and short-Circuited

### This is only a proposed re-branding!

I need to gain the [concensus](http://www.theopensourceway.org/book/The_Open_Source_Way-Stuff_everyone_knows_and_forgets_anyway-Seek_consensus_-_use_voting_as_a_last_resort.html) of the X2Go, Arctica and QVD developers 1st.

And the executables/libraries still have "nx" or "NX" in their names.

### What do you mean Caching?

By caching the X11 traffic, especially pixmaps/bitmaps, performance is greatly improved from a user's perspective.

For example, the 1st time a user opens the applications menu or opens an image, it may load a tad slowly. But subsequently opening it will be fast.

This also reduces bandwidth consumption greatly. This in turn improves performance for other users when multiple users are sharing the same WAN connection.

### What do you mean Compression?

By compressing the X11 pixmaps/bitmaps, via either lossy or lossless compression, performance is also improved for the user.

The 2 most common compression methods are JPEG (lossy) and PNG (lossless.)

Furthermore, if your system libraries (like libjpegturbo) support SIMD acceleration, then Xccc benefits from it.

This also reduces bandwidth consumption, which in turn improves performance for other users sharing the same WAN connection.

### What do you mean by short-Circuiting?
We can't tell you; that is our secret sauce!

### sudo What do you mean by short-Circuiting?
OK

Xccc eliminates most of the X11 round-trips. This improves performance, even for newer toolkits.

### But I thought that newer toolkits use XCB, and are therefore unaffected by X11 round-trips.

The use of XCB does cause them to use [fewer](https://www.youtube.com/watch?v=G0zNWswcqMg) round-trips, and be less affected by them.

Emperically, they still perform much faster when Xccc eliminates most of the round-trips.

See X.org contributor Bart Massey's [explanation](https://lwn.net/Articles/343506/) for more info.

And feel free to send a PR or patch with a (link to a) better/more detailed explanation.

### Shouldn't it be Xccsc?
We decided to short-Curcuit the s.

### Why are the executables called Xccagent and Xccproxy?
We are all about short-Circuiting!

Also, we wanted to limit their filenames to 8 characters.

### This sounds an awful like like [LBX](http://keithp.com/~keithp/talks/lbxpost/)...
Yes, however:

1. LBX never supported caching.
2. LBX never supported lossy image compression.
3. LBX never supported short-Circuiting (eliminating the round-trips).

###  This sounds an awful like like [nx-libs](https://github.com/ArcticaProject/nx-libs)...

Yes, we are rebranding nx-libs.

But there are technical changes:

1. No more bundled libraries once 3.6.0 is released! (The 3.6.x branch currently has most of them removed.)
2. We are adding new features like replacing TCP sockets with UNIX sockets.
3. Seriously, do you have any idea [how bad](http://www.theopensourceway.org/book/The_Open_Source_Way-How_to_tell_if_a_FLOSS_project_is_doomed_to_FAIL.html) bundled libraries are? Some of them were *modified* too.

The rebranding is necessary for other reasons too:

1. We do not want to be associated with NoMachine NX3. We are not just maintaining a legacy branch; we are actively developing the codebase.
2. "nx-libs" is confusing. We provide 2 executables (Xccagent and Xccproxy) in addition to the libraries.
3. We do not want people to think that they have to link against our GPLv2 code in order to use Xccc. For most users, calling Xcccagent and Xcccproxy, and possibly re-embedding them, will be sufficient.
4. We want to have fundamentally different policies to working with upstream X.org. Hopefully ["Upstream First"](http://community.redhat.com/blog/2015/03/upstream-first-turning-openstack-into-an-nfv-platform/), but we need to reach [concensus](http://www.theopensourceway.org/book/The_Open_Source_Way-Stuff_everyone_knows_and_forgets_anyway-Seek_consensus_-_use_voting_as_a_last_resort.html) on that 1st.
5. The specter of bundled libraries [still haunts](https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=655699) nx-libs.


###  This page is unprofessional!

[The day may come when we gain lots of corporate sponsors; when we forsake our wit and break all bonds of humor; but it is not this day! This day we jest!](https://youtu.be/EXGUNvIFTQw?t=24)
