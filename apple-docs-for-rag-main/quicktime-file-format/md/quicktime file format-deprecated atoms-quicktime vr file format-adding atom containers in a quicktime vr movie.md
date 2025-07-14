

- QuickTime File Format
- Deprecated atoms
- QuickTime VR file format
-  Adding atom containers in a QuickTime VR Movie 

Article

# Adding atom containers in a QuickTime VR Movie

Add node information to your QuickTime VR world.

## Overview

Assuming you have already created the QuickTime VR world and node information atom containers, you would use the code (minus error checking) in the following listing to add them to the QTVR track.

```
long descSize;
QTVRSampleDescriptionHandle qtvrSampleDesc;

// Create a  QTVR sample description handle

descSize = sizeof(QTVRSampleDescription) + GetHandleSize((Handle)  vrWorld) -
                                        sizeof(UInt32);
qtvrSampleDesc = (QTVRSampleDescriptionHandle) NewHandleClear (descSize);
(*qtvrSampleDesc)->size = descSize;
(*qtvrSampleDesc)->type = kQTVRQTVRType;

// Copy the VR world atom container data into the QTVR sample description
BlockMove (*((Handle) vrWorld), &((*qtvrSampleDesc)->data),
                            GetHandleSize((Handle) vrWorld));
// Now add it to the QTVR track's media
err = BeginMediaEdits (qtvrMedia);
err = AddMediaSample (qtvrMedia, (Handle) nodeInfo, 0,
    GetHandleSize((Handle) nodeInfo), duration,
    (SampleDescriptionHandle) qtvrSampleDesc, 1, 0, &sampleTime);
err = EndMediaEdits (qtvrMedia);
InsertMediaIntoTrack (qtvrTrack, trackTime, sampleTime, duration,  1L

The `duration` value is computed based on the duration of the corresponding image track samples for the node. The value of `trackTime` is the time for the beginning of the current node (zero for a single node movie). The values of `duration` and `sampleTime` are in the time base of the media; the value of `trackTime` is in the movie’s time base.

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

Optimizing QuickTime VR movies for web playback

Prevent having to download an entire movie before starting playback.

