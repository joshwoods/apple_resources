

- Messages
- MSStickerBrowserView
-  setContentOffset(\_:animated:) 

Instance Method

# setContentOffset(\_:animated:)

Sets the offset distance between the content and the browser’s origin.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
func setContentOffset(
    _ contentOffset: CGPoint,
    animated: Bool
)
```

## Parameters 

`contentOffset`  

The distance that the content is offset from the browser’s origin.

`animated`  

A Boolean value that determines whether the change is animated. If true, the change is animated at a constant velocity. If false, the change takes place immediately.

## Discussion

Increasing the offset’s `x` value shifts the content to the left. Increasing the offset’s `y` value shifts the content upward.

## See Also

### Managing the Browser’s Appearance

var contentInset: UIEdgeInsets

The distance that the content is inset from the edge of the browser view.

var contentOffset: CGPoint

The distance that the content is offset from the browser’s origin.

var stickerSize: MSStickerSize

The size of the stickers in the browser.

