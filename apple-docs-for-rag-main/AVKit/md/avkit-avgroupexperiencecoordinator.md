

- AVKit
-  AVGroupExperienceCoordinator 

Class

# AVGroupExperienceCoordinator

An object that synchronizes viewing environment state across participants in a SharePlay session.

visionOS 1.0+

``` source
@objc(AVGroupExperienceCoordinator)
class AVGroupExperienceCoordinator
```

## Overview

Access an experience coordinator by querying a player view controller for its groupExperienceCoordinator object.

## Topics

### Coordinating state changes

func coordinateWithSession&lt;T>(GroupSession&lt;T>)

Begins coordinating viewing environment state with a group session.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### visionOS Playback

Creating a multiview video playback experience in visionOS

Build an interface that plays multiple videos simultaneously and handles transitions to different experience types gracefully.

Adopting the system player interface in visionOS

Provide an optimized viewing experience for watching 3D video content.

Trimming and exporting media in visionOS

Display standard controls in your app to edit the timeline of the currently playing media.

class AVPlayerViewController

A view controller that displays content from a player and presents a native user interface to control playback.

protocol AVPlayerViewControllerDelegate

A protocol that defines the methods to implement to respond to player view controller events.

class AVExperienceController

An object that controls video experiences.

class AVMultiviewManager

An object that manages viewing multiple videos at once.

