

- Media Player
-  MPFeedbackCommand 

Class

# MPFeedbackCommand

An object that reflects the feedback state for the playing item.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
class MPFeedbackCommand
```

## Overview

The shared MPRemoteCommandCenter object vends feedback objects for liking, disliking, and bookmarking media items. Use these objects to register handlers for the types of feedback your app supports and to perform the appropriate tasks when that feedback changes. When the currently playing item changes, you can also use this object to set the feedback state for the new item.

When the state of a feedback item changes, the system delivers an appropriate event to registered handlers of this object. Your handler code must determine which media item receives the feedback and then apply the update the feedback state for that item. You might also perform other tasks related to receiving feedback. For example, if the user likes the currently playing song, you might update the appropriate UI in your app or use the information to recommend similar songs.

## Topics

### Retrieving information about a feedback command

var isActive: Bool

A Boolean value that indicates whether the feedback’s action is on or off.

var localizedTitle: String

A localized string used to describe the context of a command.

var localizedShortTitle: String

A shortened version of the string used to describe the context of a command.

## Relationships

### Inherits From

- MPRemoteCommand

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Responding to feedback and rating events

class MPFeedbackCommandEvent

An event requesting a change in the feedback setting.

class MPRatingCommand

An object that provides a detailed rating for the playing item.

class MPRatingCommandEvent

An event requesting a change in the rating.

