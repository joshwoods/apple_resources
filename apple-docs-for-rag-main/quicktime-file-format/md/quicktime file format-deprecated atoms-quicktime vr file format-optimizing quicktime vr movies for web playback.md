

- QuickTime File Format
- Deprecated atoms
- QuickTime VR file format
-  Optimizing QuickTime VR movies for web playback 

# Optimizing QuickTime VR movies for web playback

Prevent having to download an entire movie before starting playback.

## Overview

Originally, both QuickTime movies and QuickTime VR movies had to be completely downloaded to the user’s local hard disk before they could be viewed. Starting with QuickTime 2.5, if the movie data is properly laid out in the file, standard linear QuickTime movies can be viewed almost immediately. The frames that have been downloaded so far are shown while subsequent frames continue to be downloaded.

The important change that took place to allow this to happen was for QuickTime to place global movie information at the beginning of the file. Originally, this information was at the end of the file. After that, the frame data simply needs to be in order in the file. Similarly, QuickTime VR files also need to be laid out in a certain manner in order to get some sort of quick feedback when viewing on the web. Roughly speaking this involves writing out all of the media samples in the file in a particular order. Apple now provides a movie export component that does this for you: the QTVR Flattener.

## Topics

### Optimizations

The QTVR flattener

Optimize a movie for delivery over the web.

Sample atom container for the QTVR flattener

Specify an import preview file for the flattener with atoms.

## See Also

### Storing QuickTime VR files

Single-node panoramic movies

Store a QTVR track, a panorama track, and a panorama image track in a single-node panoramic movie.

Single-node object movies

Store a QTVR track, an object track, and an object image track in a single-node object movie.

Multinode movies

Store any number of object and panoramic nodes in a multinode QuickTime VR movie.

Getting the name of a QuickTime VR node

Retrieve information from a QuickTime VR node with QuickTime atom container functions.

Adding custom atoms in a QuickTime VR movie

Provide additional information about a QuickTime VR movie using custom atoms.

Adding atom containers in a QuickTime VR Movie

Add node information to your QuickTime VR world.

