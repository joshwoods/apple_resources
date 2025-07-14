

- Messages
- MSStickerBrowserView
-  contentInset 

Instance Property

# contentInset

The distance that the content is inset from the edge of the browser view.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
var contentInset: UIEdgeInsets { get set }
```

## Discussion

Use this property to add to the scrollable area around the content. The insets are measured in points. The default value is zero.

## See Also

### Managing the Browser’s Appearance

var contentOffset: CGPoint

The distance that the content is offset from the browser’s origin.

func setContentOffset(CGPoint, animated: Bool)

Sets the offset distance between the content and the browser’s origin.

var stickerSize: MSStickerSize

The size of the stickers in the browser.

