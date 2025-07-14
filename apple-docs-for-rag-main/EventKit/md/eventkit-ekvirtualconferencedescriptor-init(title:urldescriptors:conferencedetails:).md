

- EventKit
- EKVirtualConferenceDescriptor
-  init(title:urlDescriptors:conferenceDetails:) 

Initializer

# init(title:urlDescriptors:conferenceDetails:)

Creates an object that describes a virtual conference, including a name and URL to join the conference.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    title: String?,
    urlDescriptors URLDescriptors: [EKVirtualConferenceURLDescriptor],
    conferenceDetails: String?
)
```

## Parameters 

`title`  

The user-visible name of the virtual conference.

`URLDescriptors`  

An array that contains objects with details about where to join the virtual conference. Calendar uses the first URL descriptor as the preferred way for users to join a virtual conference, and displays additional URLs as links in the virtual conference details.

`conferenceDetails`  

Additional information about the conference that users may find helpful.

## Return Value

An object that describes a virtual conference.

