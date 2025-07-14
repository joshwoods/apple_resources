

- QuickTime File Format
- Deprecated atoms
- QuickTime VR file format
-  Getting the name of a QuickTime VR node 

Article

# Getting the name of a QuickTime VR node

Retrieve information from a QuickTime VR node with QuickTime atom container functions.

## Overview

You can use standard QuickTime atom container functions to retrieve the information in a QuickTime VR node header atom. For example, the `MyGetNodeName` function defined in the following listing returns the name of a node, given its node ID.

```
OSErr MyGetNodeName (QTVRInstance theInstance, UInt32 theNodeID,
                                                                 StringPtr  theStringPtr)
{
    OSErr                   theErr = noErr;
    QTAtomContainer         theNodeInfo;
    QTVRNodeHeaderAtomPtr   theNodeHeader;
    QTAtom                  theNodeHeaderAtom = 0;

    //Get the node information atom container.
    theErr = QTVRGetNodeInfo(theInstance, theNodeID, &theNodeInfo);

    //Get the node header atom.
    if (!theErr)
        theNodeHeaderAtom = QTFindChildByID(theNodeInfo, kParentAtomIsContainer,
                                                    kQTVRNodeHeaderAtomType,  1,  nil);
    if (theNodeHeaderAtom != 0) {
        QTLockContainer(theNodeInfo);

        //Get a pointer to the node header atom data.
        theErr = QTGetAtomDataPtr(theNodeInfo, theNodeHeaderAtom,  nil,
                                                            (Ptr  *)&theNodeHeader);
        //See if there is a name atom.
        if (!theErr && theNodeHeader->nameAtomID != 0)  {
            QTAtom theNameAtom;
            theNameAtom = QTFindChildByID(theNodeInfo, kParentAtomIsContainer,
                                kQTVRStringAtomType, theNodeHeader->nameAtomID,  nil);
            if (theNameAtom != 0) {
                VRStringAtomPtr theStringAtomPtr;

                //Get a pointer to the name atom data; copy it into  the string.
                theErr = QTGetAtomDataPtr(theNodeInfo, theNameAtom,  nil,
                                                            (Ptr  *)&theStringAtomPtr);
                if (!theErr) {
                    short theLen = theStringAtomPtr->stringLength;
                    if (theLen > 255)
                        theLen = 255;
                    BlockMove(theStringAtomPtr->string, &theStringPtr[1],  theLen);
                    theStringPtr[0] = theLen;
                }
            }
        }
        QTUnlockContainer(theNodeInfo);
    }

    QTDisposeAtomContainer(theNodeInfo);
    return(theErr);
}
```

The `MyGetNodeName` function defined in the preceeding listing retrieves the node information atom container (by calling `QTVRGetNodeInfo`) and then looks inside that container for the node header atom with atom ID `1`. If it finds one, it locks the container and then gets a pointer to the node header atom data. The desired information, the node name, is contained in the string atom whose atom ID is specified by the `nameAtomID` field of the node header structure. Accordingly, the `MyGetNodeName` function then calls `QTFindChildByID` once again to find that string atom. If the string atom is found, `MyGetNodeName` calls `QTGetAtomDataPtr` to get a pointer to the string atom data. Finally, `MyGetNodeName` copies the string data into the appropriate location and cleans up after itself before returning.

## See Also

### Storing QuickTime VR files

Single-node panoramic movies

Store a QTVR track, a panorama track, and a panorama image track in a single-node panoramic movie.

Single-node object movies

Store a QTVR track, an object track, and an object image track in a single-node object movie.

Multinode movies

Store any number of object and panoramic nodes in a multinode QuickTime VR movie.

Adding custom atoms in a QuickTime VR movie

Provide additional information about a QuickTime VR movie using custom atoms.

Adding atom containers in a QuickTime VR Movie

Add node information to your QuickTime VR world.

Optimizing QuickTime VR movies for web playback

Prevent having to download an entire movie before starting playback.

