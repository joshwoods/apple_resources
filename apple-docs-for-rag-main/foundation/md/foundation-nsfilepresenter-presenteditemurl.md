

- Foundation
- NSFilePresenter
-  presentedItemURL 

Instance Property

# presentedItemURL

The URL of the presented file or directory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var presentedItemURL: URL? { get }
```

**Required**

## Discussion

File presenters must implement this property and use it to return the file or directory of interest. If this object presents a group of related files that all reside in the same directory, specify the URL of the directory instead of creating separate presenter objects for each file. For example, a single-window application that manages multiple files inside a project directory should monitor the project directory.

The URL associated with your item may be requested by objects not associated with your presenter. Therefore, your implementation of the accessor method for this property must be thread safe and capable of running in multiple dispatch or operation queues simultaneously.

## See Also

### Accessing File Presenter Attributes

var presentedItemOperationQueue: OperationQueue

The operation queue in which to execute presenter-related messages.

**Required**

var primaryPresentedItemURL: URL?

The URL of a secondary item’s primary presented file or directory.

