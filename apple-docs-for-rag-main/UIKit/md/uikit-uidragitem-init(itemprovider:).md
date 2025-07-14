

- UIKit
- UIDragItem
-  init(itemProvider:) 

Initializer

# init(itemProvider:)

Initializes a new drag item with a specified item provider.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(itemProvider: NSItemProvider)
```

## Parameters 

`itemProvider`  

An instance of NSItemProvider that conveys the data or file to share during the drag-and-drop activity.

## Return Value

A drag item that the system initializes with the specified item provider.

## Discussion

Provide an NSItemProvider object to create a new drag item. The item provider communicates the data that the drag-and-drop activity shares between processes.

