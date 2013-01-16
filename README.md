libcork.framework
=================

Xcode project for building a framework from the [libcork](https://github.com/redjack/libcork/) sources.

Usage
-----

Add “libcork.xcodeproj” to your project (preferably into “Frameworks” to keep things tidy).

In your target’s “Build Phases”:

* Add Build Phase (+-button pull-down menu) > Copy Files
* Destination: Frameworks
* Change name to “Copy Frameworks” to keep things clean

Add “libcork.framework” to the following build phases (via the +-buttons):

* “Target Dependencies”
* “Link Binary With Libraries”
* “Copy Frameworks” (created above)

And finally add the headers you need to your code. This example will add the header for the data structures.

    #import <libcork/ds.h>

