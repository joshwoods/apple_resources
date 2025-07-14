

- EventKit
-  EKVirtualConferenceURLDescriptor 

Class

# EKVirtualConferenceURLDescriptor

Details about how users join a virtual conference, including a title and URL.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 8.0+

``` source
class EKVirtualConferenceURLDescriptor
```

## Overview

To let users join a virtual conference, you provide one or more URL descriptor objects in the EKVirtualConferenceDescriptor for the conference. Calendar uses the first URL descriptor as the preferred way for users to join a virtual conference and displays any additional links you provide in the virtual conference details.

## Topics

### Creating URL Descriptors

init(title: String?, url: URL)

Creates a URL descriptor with the given title and URL.

### Configuring URL Descriptors

var title: String?

The user-visible name of a room where virtual conferences take place, such as Personal Room or Team Room.

var url: URL

The URL that users open to join a virtual conference.

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

### Configuring Virtual Conferences

var title: String?

The user-visible name of the virtual conference.

var urlDescriptors: [EKVirtualConferenceURLDescriptor]

An array that contains objects with details about where to join the virtual conference.

var conferenceDetails: String?

Additional information about the conference that users may find helpful.

