

- EventKit
- EKVirtualConferenceDescriptor
-  conferenceDetails 

Instance Property

# conferenceDetails

Additional information about the conference that users may find helpful.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 8.0+

``` source
var conferenceDetails: String? { get }
```

## See Also

### Configuring Virtual Conferences

var title: String?

The user-visible name of the virtual conference.

var urlDescriptors: [EKVirtualConferenceURLDescriptor]

An array that contains objects with details about where to join the virtual conference.

class EKVirtualConferenceURLDescriptor

Details about how users join a virtual conference, including a title and URL.

