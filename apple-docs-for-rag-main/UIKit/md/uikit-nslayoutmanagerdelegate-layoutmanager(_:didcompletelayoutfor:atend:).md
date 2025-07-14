

- UIKit
- NSLayoutManagerDelegate
-  layoutManager(\_:didCompleteLayoutFor:atEnd:) 

Instance Method

# layoutManager(\_:didCompleteLayoutFor:atEnd:)

Informs the delegate when the layout manager finishes laying out text in the specified text container.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
optional func layoutManager(
    _ layoutManager: NSLayoutManager,
    didCompleteLayoutFor textContainer: NSTextContainer?,
    atEnd layoutFinishedFlag: Bool
)
```

## Parameters 

`layoutManager`  

The layout manager doing the layout.

`textContainer`  

The text container in which layout is complete. If `nil`, if there aren’t enough containers to hold all the text; the delegate can use this information as a cue to add another text container.

`layoutFinishedFlag`  

If true, `aLayoutManager` is finished laying out its text—this also means that `aTextContainer` is the final text container used by the layout manager. Delegates can use this information to show an indicator or background or to enable or disable a button that forces immediate layout of text.

## Discussion

This message is sent whenever a text container has been filled. This method can be useful for paginating.

## See Also

### Responding to text container layout

func layoutManager(NSLayoutManager, textContainer: NSTextContainer, didChangeGeometryFrom: CGSize)

Informs the delegate when the layout manager invalidates layout due to a change in the geometry of the specified text container.

