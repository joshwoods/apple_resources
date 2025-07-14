

- AppKit
- NSTextContainer
-  layoutManager 

Instance Property

# layoutManager

The text container’s layout manager.

macOS 10.0+

``` source
unowned(unsafe) var layoutManager: NSLayoutManager? { get set }
```

## Discussion

Avoid assigning a layout manager directly through this property. Instead, use the replaceLayoutManager(_:) method when you want to replace the layout manager. The framework sets the value of this property automatically when you add a text container to your layout manager using the addTextContainer(_:) method.

## See Also

### Managing text components

var textLayoutManager: NSTextLayoutManager?

func replaceLayoutManager(NSLayoutManager)

Replaces the layout manager for the group of text system objects that contains the text container.

var textView: NSTextView?

The text container’s text view.

