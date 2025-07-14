

- Foundation
- NSFileCoordinator
-  removeFilePresenter(\_:) 

Type Method

# removeFilePresenter(\_:)

Unregisters the specified file presenter object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func removeFilePresenter(_ filePresenter: any NSFilePresenter)
```

## Parameters 

`filePresenter`  

The file presenter object to unregister. If the object is not currently registered, this method does nothing.

## Discussion

Call this method to unregister file presenters before those objects are deallocated, even in a garbage-collected application.

## See Also

### Managing File Presenters

class func addFilePresenter(any NSFilePresenter)

Registers the specified file presenter object so that it can receive notifications.

class var filePresenters: [any NSFilePresenter]

Returns an array containing the currently registered file presenter objects.

var purposeIdentifier: String

A string that uniquely identifies the file access that was performed by this file coordinator.

