

- Messages
- MSStickerBrowserView
-  contentOffset 

Instance Property

# contentOffset

The distance that the content is offset from the browser’s origin.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
var contentOffset: CGPoint { get set }
```

## Discussion

Positive `x` values shift the content to the left. Positive `y` values shift the content upward. The default value is CGPointZero.

## See Also

### Managing the Browser’s Appearance

var contentInset: UIEdgeInsets

The distance that the content is inset from the edge of the browser view.

func setContentOffset(CGPoint, animated: Bool)

Sets the offset distance between the content and the browser’s origin.

var stickerSize: MSStickerSize

The size of the stickers in the browser.

