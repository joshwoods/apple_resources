

- AppKit
- NSClipView
-  copiesOnScroll Deprecated

Instance Property

# copiesOnScroll

A Boolean value that indicates if the clip view copies rendered images while scrolling.

macOS 10.0–11.0Deprecated

``` source
@MainActor
var copiesOnScroll: Bool { get set }
```

Deprecated

Setting this property has no effect. NSClipView will always minimize the area of the document view that is invalidated. To force invalidation of the document view, use -\[NSView setNeedsDisplayInRect:\].

## Discussion

When the value of this property is true, the clip view copies its existing rendered image while scrolling (only drawing exposed portions of its document view); when it is false, the view forces its contents to be redrawn each time.

