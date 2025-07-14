

- QuickTime File Format
- Deprecated atoms
-  Support for wired actions 

Article

# Support for wired actions

Support wired actions in a QuickTime VR file.

## Overview

Important

VR Media is deprecated in the QuickTime file format. The information that follows documents existing content containing VR Media and should not be used for new development.

Certain actions on a QuickTime VR movie can trigger wired actions if the appropriate event handler atoms have been added to the file. This section discusses what atoms must be included in the QuickTime VR file to support wired actions.

As with sprite tracks, the presence of a certain atom in the media property atom container of the QTVR track enables the handling of wired actions. This atom is of type `kSpriteTrackPropertyHasActions`, which has a single Boolean value that must be set to `true`.

When certain events occur and the appropriate event handler atom is found in the QTVR file, then that atom is passed to QuickTime to perform any actions specified in the atom. The event handler atoms themselves must be added to the node information atom container in the QTVR track. There are two types of event handlers for QTVR nodes: global and hot spot specific. The currently supported global event handlers are `kQTEventFrameLoaded` and `kQTEventIdle`. The event handler atoms for these are located at the root level of the node information atom container. A global event handler atom’s type is set to the event type and its ID is set to `1`.

Hot spot–specific event handler atoms are located in the specific hot spot atom as a sibling to the hot spot info atom. For these atoms, the atom type is always `kQTEventType` and the ID is the `event` type. Supported hot spot–specific event types are `kQTEventMouseClick`, `kQTEventMouseClickEnd`, `kQTEventMouseClickEndTriggerButton`, and `kQTEventMouseEnter`, `kQTEventMouseExit`.

The specific actions that cause these events to be generated are described as follows:

`kQTEventFrameLoaded` (`'fram'`)  
A wired action that is generated when a node is entered, before any application-installed entering-node procedure is called (this event processing is considered part of the node setup that occurs before the application’s routine is called).

`kQTEventIdle` (`'idle'`)  
A wired action that is generated every `n` ticks, where `n` is defined by the contents of the `kSpriteTrackPropertyQTIdleEventsFrequency` atom (`SInt32`) in the media property atom container. When appropriate, this event is triggered before any normal idle processing occurs for the QuickTime VR movie.

`kQTEventMouseClick` (`'clik'`)  
A wired action that is generated when the mouse goes down over a hot spot.

`kQTEventMouseClickEnd` (`'cend'`)  
A wired action that is generated when the mouse goes up after a `kQTEventMouseClick` is generated, regardless of whether the mouse is still over the hot spot originally clicked. This event occurs prior to QuickTime VR’s normal mouse-up processing.

`kQTEventMouseClickEndTriggerButton` (`'trig'`)  
A wired action that is generated when a click end triggers a hot spot (using the same criterion as used by QuickTime VR in 2.1 for link/url hot spot execution). This event occurs prior to QuickTime VR’s normal hot spot–trigger processing.

`kQTEventMouseEnter` (`'entr'`), `kQTEventMouseExit`(`'exit'`)  
Wired action that are generated when the mouse rolls into or out of a hot spot, respectively. These events occur whether or not the mouse is down and whether or not the movie is being panned. These events occur after any application-installed `MouseOverHotSpotProc` is called, and will be cancelled if the return value from the application’s routine indicates that QuickTimeVR’s normal over–hot spot processing should not take place.

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

