

- UIKit
- UITextPasteItem
-  localObject 

Instance Property

# localObject

The custom local object that the copy or drag source optionally attached to the drag item.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var localObject: Any? { get }
```

**Required**

## Discussion

The local object is available only to the app that initiates the copy or drag activity.

## See Also

### Accessing the text paste item’s data

var itemProvider: NSItemProvider

The item provider for the item being pasted or dropped.

**Required**

