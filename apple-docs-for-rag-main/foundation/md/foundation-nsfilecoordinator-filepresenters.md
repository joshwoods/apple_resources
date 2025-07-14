

- Foundation
- NSFileCoordinator
-  filePresenters 

Type Property

# filePresenters

Returns an array containing the currently registered file presenter objects.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var filePresenters: [any NSFilePresenter] { get }
```

## Return Value

An array of objects that conform to the NSFilePresenter protocol.

## See Also

### Managing File Presenters

class func addFilePresenter(any NSFilePresenter)

Registers the specified file presenter object so that it can receive notifications.

class func removeFilePresenter(any NSFilePresenter)

Unregisters the specified file presenter object.

var purposeIdentifier: String

A string that uniquely identifies the file access that was performed by this file coordinator.

