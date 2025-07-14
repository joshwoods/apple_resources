

- WatchKit
- WKVideoGravity
-  WKVideoGravity.resizeAspectFill 

Case

# WKVideoGravity.resizeAspectFill

Content is resized to fill the bounds rectangle completely while preserving the original aspect ratio of the content. This option results in cropping of the edges of the video in the axis it exceeds.

watchOS 2.0+

``` source
case resizeAspectFill
```

## See Also

### Constants

case resizeAspect

Content is resized to fit the bounds rectangle, preserving the original aspect ratio of the content. Content that does not completely fill the bounds rectangle is centered in the partial axis.

case resize

Content is resized to fit the entire bounds rectangle. This option does not preserve the original aspect ratio of the content.

