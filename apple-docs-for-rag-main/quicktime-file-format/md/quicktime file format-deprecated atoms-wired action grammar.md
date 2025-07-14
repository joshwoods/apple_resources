

- QuickTime File Format
- Deprecated atoms
-  Wired action grammar 

Article

# Wired action grammar

Embed QT event handlers in their media samples.

## Overview

The wired action grammar shown in this section allows QT event handlers to be expressed in a QuickTime movie. The sprite, text, VR, 3D, and Flash media handlers all support the embedding of QT event handlers in their media samples.

```
[(ActionListAtoms)] =
    kAction, (anyUniqueIDs), (1..numActions)
        kWhichAction    1, 1
            [long whichActionConstant]
          (anyUniqueIDs), (1..numParameters)
            [(parameterData)] ( whichActionConstant, paramIndex  )
    // either leaf data or child atoms
          parameterID,  (1..numParamsWithFlags)
            [long actionFlags]
          parameterID,  (1.. numParamsWithMin)
            [data depends on param type]
          parameterID,  (1.. numParamsWithMax)
            [data depends on param type]
        [(ActionTargetAtoms)]

        , (anyUniqueIDs), (1..numComments)
            [CString]

[(ActionTargetAtoms)] =

            [no data]

        [IDlong childMovieTrackID]

            [long childMovieTrackIndex]

            [PString childMovieName]

            [long childMovieID]

            [PString trackName]

            [OSType trackType]

            [long trackIndex]
            OR
            [(kExpressionAtoms)]

            [long trackID]
            OR
            [(kExpressionAtoms)]

            [PString spriteName]

            [short spriteIndex]
            OR
            [(kExpressionAtoms)]

            [QTAtomID spriteIID]
            OR
            [(kExpressionAtoms)]

            [CString objectName]

[(kExpressionAtoms)] =
    kExpressionContainerAtomType, 1, 1

            kOperandAtomType, (anyUniqueIDs), (1..numOperands)
                [(OperandAtoms)]
        OR

            [(OperandAtoms)]
[(ActionTargetAtoms)] =

            [Pstring MovieName]
        OR

            [long MovieID]
            OR
            [(kExpressionAtoms)]

[(OperandAtoms)] =
     1, 1
        [(kExpressionAtoms)]        // allows for recursion
    OR
     1, 1
        [ float theConstant ]
    OR
     1, 1
        [(ActionTargetAtoms)]
        kActionParameter, 1, 1
            [QTAtomID spriteVariableID]
    OR
     1, 1
        kActionParameter, 1, 1
            [UInt16 modifierKeys]
        kActionParameter, 2, 2
            [UInt8 asciiCharCode]
    OR
     1, 1
        kActionParameter, 1, 1
            [short minimum]
        kActionParameter, 2, 2
            [short maximum]
    OR

        [(ActionTargetAtoms)]
```

The format for parameter data depends on the action and parameter index.

In most cases, the `kActionParameter` atom is a leaf atom containing data; for a few parameters, it contains child atoms.

`whichAction` corresponds to the action type that is specified by the leaf data of a `kWhichAction` atom.

`paramIndex` is the index of the parameter’s `kActionParameter` atom.

```
[(parameterData)] ( whichAction, paramIndex ) =
{
    kActionMovieSetVolume:
        param1:     short volume

    kActionMovieSetRate
        param1:     Fixed rate

    kActionMovieSetLoopingFlags
        param1:     long loopingFlags

    kActionMovieGoToTime
        param1:     TimeValue time

    kActionMovieGoToTimeByName
        param1:     Str255 timeName

    kActionMovieGoToBeginning
        no params

    kActionMovieGoToEnd
        no params

    kActionMovieStepForward
        no params

    kActionMovieStepBackward
        no params

    kActionMovieSetSelection
        param1:     TimeValue startTime
        param2:     TimeValue endTime

    kActionMovieSetSelectionByName
        param1:     Str255 startTimeName
        param2:     Str255 endTimeName

    kActionMoviePlaySelection
        param1:     Boolean selectionOnly

    kActionMovieSetLanguage
        param1:     long language

    kActionMovieChanged
        no params

    kActionTrackSetVolume
        param1:     short volume

    kActionTrackSetBalance
        param1:     short balance

    kActionTrackSetEnabled
        param1:     Boolean enabled

    kActionTrackSetMatrix
        param1:     MatrixRecord matrix

    kActionTrackSetLayer
        param1:     short layer

    kActionTrackSetClip
        param1:     RgnHandle clip

    kActionSpriteSetMatrix
        param1:     MatrixRecord matrix

    kActionSpriteSetImageIndex
        parm1:      short imageIndex

    kActionSpriteSetVisible
        param1:     short visible

    kActionSpriteSetLayer
        param1:     short layer

    kActionSpriteSetGraphicsMode
        param1:     ModifierTrackGraphicsModeRecord graphicsMode

    kActionSpritePassMouseToCodec
        no params

    kActionSpriteClickOnCodec
        param1:     Point localLoc

    kActionSpriteTranslate
        param1:     Fixed x
        param2:     Fixed y
        param3:     Boolean isRelative

    kActionSpriteScale
        param1:     Fixed xScale
        param2:     Fixed yScale

    kActionSpriteRotate
        param1:     Fixed degrees

    kActionSpriteStretch
        param1:     Fixed p1x
        param2:     Fixed p1y
        param3:     Fixed p2x
        param4:     Fixed p2y
        param5:     Fixed p3x
        param6:     Fixed p3y
        param7:     Fixed p4x
        param8:     Fixed p4y

    kActionQTVRSetPanAngle
        param1:     float panAngle

    kActionQTVRSetTiltAngle
        param1:     float tileAngle

    kActionQTVRSetFieldOfView
        param1:     float fieldOfView

    kActionQTVRShowDefaultView
        no params

    kActionQTVRGoToNodeID
        param1:     UInt32 nodeID

    kActionMusicPlayNote
        param1:     long sampleDescIndex
        param2:     long partNumber
        param3:     long delay
        param4:     long pitch
        param5:     long velocity
        param6:     long duration

    kActionMusicSetController
        param1:     long sampleDescIndex
        param2:     long partNumber
        param3:     long delay
        param4:     long controller
        param5:     long value

    kActionCase
        param1:     [(CaseStatementActionAtoms)]

    kActionWhile
        param1:     [(WhileStatementActionAtoms)]

    kActionGoToURL
        param1:     CString urlLink

    kActionSendQTEventToSprite
        param1:     [(SpriteTargetAtoms)]
        param2:     QTEventRecord theEvent

    kActionDebugStr
        param1:     Str255 theMessageString

    kActionPushCurrentTime
        no params

    kActionPushCurrentTimeWithLabel
        param1:     Str255 theLabel

    kActionPopAndGotoTopTime
        no params

    kActionPopAndGotoLabeledTime
        param1:     Str255 theLabel

    kActionSpriteTrackSetVariable
        param1:     QTAtomID variableID
        param2:     float value

    kActionApplicationNumberAndString
        param1:     long aNumber
        param2:     Str255 aString
}
```

Both \[(CaseStatementActionAtoms)\] and \[(WhileStatementActionAtoms)\] are child atoms of a `kActionParameter 1, 1` atom.

```
[(CaseStatementActionAtoms)] =
    kConditionalAtomType, (anyUniqueIDs), (1..numCases)
        [(kExpressionAtoms)]
        kActionListAtomType 1, 1
            [(ActionListAtoms)] // may contain nested conditional  actions

[(WhileStatementActionAtoms)] =
    kConditionalAtomType, 1, 1
        [(kExpressionAtoms)]
        kActionListAtomType 1, 1
            [(ActionListAtoms)] // may contain nested conditional  actions
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

Sprite media handler sample QT atom container formats

Set sprite media handlers in QT atom containers.

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

