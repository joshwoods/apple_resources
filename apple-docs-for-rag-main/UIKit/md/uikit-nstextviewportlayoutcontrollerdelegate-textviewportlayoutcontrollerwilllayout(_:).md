

- UIKit
- NSTextViewportLayoutControllerDelegate
-  textViewportLayoutControllerWillLayout(\_:) 

Instance Method

# textViewportLayoutControllerWillLayout(\_:)

The method the framework calls before the text viewport layout controller starts its layout process.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
optional func textViewportLayoutControllerWillLayout(_ textViewportLayoutController: NSTextViewportLayoutController)
```

## Parameters 

`textViewportLayoutController`  

The NSTextViewportLayoutController.

## See Also

### Responding to changes in the viewport

func textViewportLayoutController(NSTextViewportLayoutController, configureRenderingSurfaceFor: NSTextLayoutFragment)

The method the framework calls when the layout controller lays out a text layout fragment in the UI.

**Required**

func textViewportLayoutControllerDidLayout(NSTextViewportLayoutController)

The method the framework calls when the text viewport layout controller finishes its layout process.

func viewportBounds(for: NSTextViewportLayoutController) -> CGRect

Returns the current viewport, which is the view visible bounds plus the overdraw area.

**Required**

