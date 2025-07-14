

- UIKit
- NSLayoutManager
-  textStorage 

Instance Property

# textStorage

The text storage object that contains the content to lay out.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
unowned(unsafe) var textStorage: NSTextStorage? { get set }
```

## See Also

### Related Documentation

func addLayoutManager(NSLayoutManager)

Adds a layout manager to the text storage object’s set of layout managers.

### Accessing the text storage

func replaceTextStorage(_ newTextStorage: NSTextStorage)

Replaces the layout manager’s current text storage object with the specified object.

