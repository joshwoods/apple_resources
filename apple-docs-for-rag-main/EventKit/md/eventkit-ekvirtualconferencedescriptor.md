

- EventKit
-  EKVirtualConferenceDescriptor 

Class

# EKVirtualConferenceDescriptor

Details about a virtual conference that uses a custom room type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 8.0+

``` source
class EKVirtualConferenceDescriptor
```

## Overview

When users add events to their calendars and use one of the room types that your provider defines, EventKit requests a virtual conference descriptor from your provider. Each virtual conference descriptor contains:

- A user-visible name for the virtual conference

- One or more URLs that the users open to join the virtual conference

- Optional details about the conference that may be helpful to users

Calendar uses the first URL that you provide as the preferred way for users to join a virtual conference and displays additional URLs as links in the virtual conference details.

Important

Events that use your virtual conference descriptors may sync to other devices where your app isn’t installed. To support links to your virtual conference regardless of whether your app is installed, adopt universal links in your app. Universal links let you specify HTTP URLs that open your app if it’s installed or open a corresponding web page if it’s not. For more information about adopting universal links in your app, see Supporting universal links in your app.

## Topics

### Creating Conference Descriptors

init(title: String?, urlDescriptors: [EKVirtualConferenceURLDescriptor], conferenceDetails: String?)

Creates an object that describes a virtual conference, including a name and URL to join the conference.

### Configuring Virtual Conferences

var title: String?

The user-visible name of the virtual conference.

var urlDescriptors: [EKVirtualConferenceURLDescriptor]

An array that contains objects with details about where to join the virtual conference.

class EKVirtualConferenceURLDescriptor

Details about how users join a virtual conference, including a title and URL.

var conferenceDetails: String?

Additional information about the conference that users may find helpful.

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

### Virtual conferences

class EKVirtualConferenceProvider

An object that associates virtual conferencing details with an event object in a user’s calendar.

class EKVirtualConferenceRoomTypeDescriptor

Details about a room where virtual conferences take place.

