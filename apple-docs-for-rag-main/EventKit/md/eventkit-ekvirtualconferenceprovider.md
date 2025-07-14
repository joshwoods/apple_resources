

- EventKit
-  EKVirtualConferenceProvider 

Class

# EKVirtualConferenceProvider

An object that associates virtual conferencing details with an event object in a user’s calendar.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 8.0+

``` source
class EKVirtualConferenceProvider
```

## Overview

EKVirtualConferenceProvider lets apps that offer virtual conferencing services to integrate directly with events in users’ calendars. To add this support to your app, add a virtual conference extension. The principal class of the app extension is a custom subclass of EKVirtualConferenceProvider that you create that provides the following:

- A list of room types where events take place, such as Personal Room or Team Room

- A descriptor for a virtual conference, including a user-visible title, one or more URLs, and additional details

### Providing Room Details

To provide a list of rooms, you provide one or more *room type descriptors* that contain details about where a virtual conference takes place. Each room type descriptor includes a user-visible title and an identifier that you choose. EventKit calls fetchAvailableRoomTypes(completionHandler:) on your virtual conference provider to retrieve an array of EKVirtualConferenceRoomTypeDescriptor objects.

### Providing Conference Details

After EventKit has the room type descriptors, users can add an event that specifies one of your rooms as the location. To identify the virtual conference event, your virtual conference provider creates a *virtual conference descriptor* that contains details about the virtual conference. The conference descriptor contains the following:

- One or more EKVirtualConferenceURLDescriptor objects to specify how the user joins the virtual conference

- An optional user-visible title that EventKit may display

- An optional user-visible string with details about the virtual conference that EventKit displays

EventKit calls fetchVirtualConference(identifier:completionHandler:) on your virtual conference provider to retrieve an instance of EKVirtualConferenceDescriptor.

Important

Events that use your virtual conference descriptors may sync to other devices where your app isn’t installed. To support links to your virtual conference regardless of whether your app is installed, adopt universal links in your app. Universal links let you specify HTTP URLs that open your app if it’s installed or open a corresponding web page if it’s not. For more information about adopting universal links in your app, see Supporting universal links in your app.

## Topics

### Providing Rooms

func fetchAvailableRoomTypes(completionHandler: ([EKVirtualConferenceRoomTypeDescriptor]?, (any Error)?) -> Void)

Provides an array of room types where events take place.

### Providing Virtual Conferences

func fetchVirtualConference(identifier: EKVirtualConferenceRoomTypeIdentifier, completionHandler: (EKVirtualConferenceDescriptor?, (any Error)?) -> Void)

Provides details about a virtual conference that takes place in a room the user selects.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSExtensionRequestHandling
- NSObjectProtocol

## See Also

### Virtual conferences

class EKVirtualConferenceDescriptor

Details about a virtual conference that uses a custom room type.

class EKVirtualConferenceRoomTypeDescriptor

Details about a room where virtual conferences take place.

