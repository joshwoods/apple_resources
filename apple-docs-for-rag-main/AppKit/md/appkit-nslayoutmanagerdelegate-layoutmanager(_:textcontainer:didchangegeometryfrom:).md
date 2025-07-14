

- AppKit
- NSLayoutManagerDelegate
-  layoutManager(\_:textContainer:didChangeGeometryFrom:) 

Instance Method

# layoutManager(\_:textContainer:didChangeGeometryFrom:)

Informs the delegate when the layout manager invalidates layout due to a change in the geometry of the specified text container.

macOS 10.11+

``` source
optional func layoutManager(
    _ layoutManager: NSLayoutManager,
    textContainer: NSTextContainer,
    didChangeGeometryFrom oldSize: NSSize
)
```

## Parameters 

`layoutManager`  

The layout manager invalidating layout.

`textContainer`  

The text container that changed geometry.

`oldSize`  

The size of the text container before it changed geometry.

## Discussion

The delegate can react to the geometry change and perform adjustments such as recreating an exclusion path.

## See Also

### Responding to text container layout

func layoutManager(NSLayoutManager, didCompleteLayoutFor: NSTextContainer?, atEnd: Bool)

Informs the delegate when the layout manager finishes laying out text in the specified text container.

