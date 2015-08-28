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

The use of XCB causes them to use [fewer](https://www.youtube.com/watch?v=G0zNWswcqMg) round-trips, and be less affected by them.

However, emperically, they still perform much faster because of the Xccc eliminates most of the round-trips.

See X.org contributor Bart Massey's [explanation](https://lwn.net/Articles/343506/) for more info.

And feel free to send a PR or patch with a (link to a) better/more detailed explanation.

### Shouldn't it be Xccsc?
We decided to short-Curcuit the s.

### Why are the executables called Xccagent and Xccproxy?
We are all about short-Circuiting!

Also, we wanted to limit their filenames to 8 characters.
