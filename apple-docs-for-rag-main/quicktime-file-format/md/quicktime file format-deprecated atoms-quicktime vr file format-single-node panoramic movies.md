

- QuickTime File Format
- Deprecated atoms
- QuickTime VR file format
-  Single-node panoramic movies 

Article

# Single-node panoramic movies

Store a QTVR track, a panorama track, and a panorama image track in a single-node panoramic movie.

## Overview

Every panoramic movie contains at least three tracks: a QTVR track, a panorama track, and a panorama image track.

For a single-node panoramic movie, the QTVR track contains just one sample. There is a corresponding sample in the panorama track, whose time and duration are the same as the time and duration of the sample in the QTVR track. The time base of the movie is used to locate the proper video samples in the panorama image track. For a panoramic movie, the video sample for the first diced frame of a node’s panoramic image is located at the same time as the corresponding QTVR and panorama track samples. The total duration of all the video samples is the same as the duration of the corresponding QTVR sample and the panorama sample.

A panoramic movie can contain an optional hot spot image track and any number of standard QuickTime tracks. A panoramic movie can also contain panoramic image tracks with a lower resolution. The video samples in these low-resolution image tracks must be located at the same time and must have the same total duration as the QTVR track. Likewise, the video samples for a hot spot image track, if one exists, must be located at the same time and must have the same total duration as the QTVR track.

## See Also

### Storing QuickTime VR files

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

Optimizing QuickTime VR movies for web playback

Prevent having to download an entire movie before starting playback.

