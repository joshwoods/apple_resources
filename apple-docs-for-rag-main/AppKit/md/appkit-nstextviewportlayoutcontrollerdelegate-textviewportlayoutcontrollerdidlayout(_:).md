

- AppKit
- NSTextViewportLayoutControllerDelegate
-  textViewportLayoutControllerDidLayout(\_:) 

Instance Method

# textViewportLayoutControllerDidLayout(\_:)

The method the framework calls when the text viewport layout controller finishes its layout process.

macOS 12.0+

``` source
optional func textViewportLayoutControllerDidLayout(_ textViewportLayoutController: NSTextViewportLayoutController)
```

## Parameters 

`textViewportLayoutController`  

The NSTextViewportLayoutController.

## Discussion

Layout information on `textViewportLayoutController` is up-to-date at the point of this call.

## See Also

### Responding to changes in the viewport

func textViewportLayoutController(NSTextViewportLayoutController, configureRenderingSurfaceFor: NSTextLayoutFragment)

The method the framework calls when the layout controller lays out a text layout fragment in the UI.

**Required**

func textViewportLayoutControllerWillLayout(NSTextViewportLayoutController)

The method the framework calls before the text viewport layout controller starts its layout process.

func viewportBounds(for: NSTextViewportLayoutController) -> CGRect

Returns the current viewport, which is the view visible bounds plus the overdraw area.

**Required**

