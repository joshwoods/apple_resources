

- QuickTime File Format
- Deprecated atoms
-  Sprite media handler sample QT atom container formats 

Article

# Sprite media handler sample QT atom container formats

Set sprite media handlers in QT atom containers.

## Overview

Important

Sprite media is deprecated in the QuickTime file format. The information that follows documents existing content containing sprite media and should not be used for new development.

```
[(SpriteKeySample)] =
    [(SpritePropertyAtoms)]
    [(SpriteImageAtoms)]

[(SpriteOverrideSample)] =
    [(SpritePropertyAtoms)]

[(SpriteImageAtoms)]
    kSpriteSharedDataAtomType, 1, 1
        , 1
            , (1..n) ID is  SpriteTrack
                            Variable ID to be set
                                                [CString]
            , (1..n)  ID is
                            SpriteTrack Variable ID to be set
                                                [float]

        kSpriteImagesContainerAtomType, 1, 1
            kSpriteImageAtomType, theImageID, (1 .. numImages)
                kSpriteImageDataAtomType, 1, 1
                    [ImageData is ImageDescriptionHandle prepended  to
                                                            image  data]

                    [FixedPoint]

                    [pString]

                    [long]

[(SpritePropertyAtoms)]
    , 1, 1
        [(ActionListAtoms)]
        , (anyUniqueIDs), (1..numComments)
            [CString]

    kSpriteAtomType, theSpriteID, (1 .. numSprites)

            [MatrixRecord]

            [short]

            [short]

            [short]

            [ModifierTrackGraphicsModeRecord]

            [array of QTAtomID's, one per image used]

        , 1

            [QTSpriteButtonBehaviorStruct]

            [QTSpriteButtonBehaviorStruct]

            [QTSpriteButtonBehaviorStruct]

[(SpriteActionAtoms)] =
    kQTEventType, theQTEventType, (1 .. numEventTypes)
            [(ActionListAtoms)] //see the next section Wired Action
                                //Grammar for a description
            , (anyUniqueIDs), (1..numComments)
                [CString]
```

## See Also

### Media data atom types

Sprite media

Sprite media is used to store character-based animation data in QuickTime movies.

Sprite track properties

Define properties that apply to an entire sprite track.

Sprite track media format

A media format for that stores sprite track information in atoms.

Sprite media atom and data types

Atoms that represent sprite media and data types.

Sprite button behaviors

Specify simple button behaviors for sprites in a sprite track.

QT atom container description key

Build QT atom container-based data structures.

Sprite media handler track properties QT atom container format

Set sprite media handler track properties in a QT atom container.

Wired action grammar

Embed QT event handlers in their media samples.

Tween media

Store pairs of values to be interpolated between in QuickTime movies using tween media.

3D media

Store 3D image data in a base media in QuickTime movies.

VR media

Atoms that describe the QuickTime VR world.

Node parent atom

An atom that is the parent of one or more node ID atoms.

Node location atom structure ('nloc')

An atom that describes the type of a node and its location.

Deprecated

Custom cursor atom

An atom you use to replace the default cursors used by QuickTime VR.

Node information atom container

An atom container that includes general information about the node such as the node’s type, ID, and name.

