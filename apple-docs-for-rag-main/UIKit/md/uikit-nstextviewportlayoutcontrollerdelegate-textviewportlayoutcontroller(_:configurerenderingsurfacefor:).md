

- UIKit
- NSTextViewportLayoutControllerDelegate
-  textViewportLayoutController(\_:configureRenderingSurfaceFor:) 

Instance Method

# textViewportLayoutController(\_:configureRenderingSurfaceFor:)

The method the framework calls when the layout controller lays out a text layout fragment in the UI.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func textViewportLayoutController(
    _ textViewportLayoutController: NSTextViewportLayoutController,
    configureRenderingSurfaceFor textLayoutFragment: NSTextLayoutFragment
)
```

**Required**

## Parameters 

`textViewportLayoutController`  

The `NSTextViewportLayoutController` associated with this text layout fragment.

`textLayoutFragment`  

An `NSTextLayoutFragment`.

## Discussion

The delegate presents the text layout fragment in the UI, for example, in a sublayer or a subview. Layout information such as `viewportBounds` on `textViewportLayoutController` isn’t up to date at the point of this call.

## See Also

### Responding to changes in the viewport

func textViewportLayoutControllerDidLayout(NSTextViewportLayoutController)

The method the framework calls when the text viewport layout controller finishes its layout process.

func textViewportLayoutControllerWillLayout(NSTextViewportLayoutController)

The method the framework calls before the text viewport layout controller starts its layout process.

func viewportBounds(for: NSTextViewportLayoutController) -> CGRect

Returns the current viewport, which is the view visible bounds plus the overdraw area.

**Required**

