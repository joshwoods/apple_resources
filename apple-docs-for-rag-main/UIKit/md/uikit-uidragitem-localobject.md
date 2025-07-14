

- UIKit
- UIDragItem
-  localObject 

Instance Property

# localObject

A custom object associated with the drag item.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var localObject: Any? { get set }
```

## Mentioned in 

Supporting drag and drop in table views

Supporting Drag and Drop in Collection Views

## Discussion

The `localObject` property gives you the option to associate a custom object, such as a model object, with the drag item. The local object is available only to the app that initiates the drag activity.

## See Also

### Accessing the drag item’s data

var itemProvider: NSItemProvider

The item provider associated with the drag item.

