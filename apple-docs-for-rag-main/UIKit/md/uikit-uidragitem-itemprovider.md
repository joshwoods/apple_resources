

- UIKit
- UIDragItem
-  itemProvider 

Instance Property

# itemProvider

The item provider associated with the drag item.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var itemProvider: NSItemProvider { get }
```

## Mentioned in 

Supporting drag and drop in table views

Supporting Drag and Drop in Collection Views

## Discussion

The item provider conveys the data, or file, that the drag-and-drop activity shares between processes. The property is set when the UIDragItem instance is created. For more information, see init(itemProvider:).

## See Also

### Accessing the drag item’s data

var localObject: Any?

A custom object associated with the drag item.

