

- Media Player
- MPMoviePlayerController
-  backgroundView Deprecated

Instance Property

# backgroundView

A customizable view that is displayed behind the movie content.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var backgroundView: UIView! { get }
```

Deprecated

Use AVPlayerViewController in AVKit

## Discussion

This view provides the backing content, on top of which the movie content is displayed. You can add subviews to the background view if you want to display custom background content.

This view is part of the view hierarchy returned by the view property.

## See Also

### Accessing the view

var view: UIView!

The view containing the movie content and controls.

Deprecated

