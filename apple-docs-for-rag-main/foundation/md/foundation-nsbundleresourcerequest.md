

- Foundation
-  NSBundleResourceRequest 

Class

# NSBundleResourceRequest

A resource manager you use to download content hosted on the App Store at the time your app needs it.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSBundleResourceRequest
```

## Overview

You identify on-demand resources during development by creating string identifiers known as tags and assigning one or more tags to each resource. An NSBundleResourceRequest object manages the resources marked by one or more tags.

You use the resource request to inform the system when the managed tags are needed and when you have finished accessing them. The resource request manages the downloading of any resources marked with the managed tags that are not already on the device and informs your app when the resources are ready for use.

Note

This class ignores calls from Mac apps built with Mac Catalyst.

The system will not attempt to purge the resources marked with a tag from on-device storage as long as at least one NSBundleResourceRequest object is managing the tag. Apps can access resources after the completion handler of either beginAccessingResources(completionHandler:) or conditionallyBeginAccessingResources(completionHandler:) is called successfully. Management ends after a call to endAccessingResources() or after the resource request object is deallocated.

Other properties and methods let you track the progress of a download, change the priority of a download, and check whether the resources marked by a set of tags are already on the device. Methods in Bundle indicate to the system the relative importance of preserving a tag in memory after it is no longer in use. For more information, see setPreservationPriority(_:forTags:) and preservationPriority(forTag:).

Important

An NSBundleResourceRequest object can only be used for one successful resource request.

## Topics

### Initializing a Resource Request

convenience init(tags: Set&lt;String>)

Initializes a resource request for managing the on-demand resources marked with any of the set of specified tags. The managed resources are loaded into the main bundle.

init(tags: Set&lt;String>, bundle: Bundle)

Initializes a resource request for managing the on-demand resources marked with any of the set of specified tags. The managed resources are loaded into the specified bundle.

### Accessing the Configuration

var bundle: Bundle

A reference to the bundle used for storing the downloaded resources. (read-only)

var tags: Set&lt;String>

A set of strings, with each string specifying a tag used to mark on-demand resources managed by the request. (read-only)

### Requesting Resources

func beginAccessingResources(completionHandler: ((any Error)?) -> Void)

Requests access to the resources marked with the managed tags. If any of the resources are not on the device, they are requested from the App Store.

func conditionallyBeginAccessingResources(completionHandler: (Bool) -> Void)

Checks whether the resources marked with the tags managed by the request are already on the device. If all of the resources are on the device, you can begin accessing those resources.

func endAccessingResources()

Informs the system that you have finished accessing the resources marked with the tags managed by the request.

### Setting the Download Priority

var loadingPriority: Double

A hint to the system of the relative priority of the resource request.

let NSBundleResourceRequestLoadingPriorityUrgent: Double

### Tracking Progress

var progress: Progress

A reference to the progress object associated with the specified resource request. (read-only)

### Errors

var NSBundleErrorMaximum: Int

The end of the range of error codes reserved for bundle errors.

var NSBundleErrorMinimum: Int

The start of the range of error codes reserved for bundle errors.

var NSBundleOnDemandResourceExceededMaximumSizeError: Int

The application exceeded the amount of on-demand resources content in use at one time.

var NSBundleOnDemandResourceInvalidTagError: Int

The application specified a tag that the system couldn’t find in the application tag manifest.

var NSBundleOnDemandResourceOutOfSpaceError: Int

Insufficient space available to download the requested on-demand resources.

### Notifications

static let NSBundleResourceRequestLowDiskSpace: NSNotification.Name

Posted after the system detects that the amount of available disk space is getting low. The notification is posted to the default notification center.

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
- ProgressReporting

