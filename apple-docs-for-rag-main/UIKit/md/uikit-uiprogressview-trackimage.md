

- UIKit
- UIProgressView
-  trackImage 

Instance Property

# trackImage

An image to use for the portion of the track that isn’t filled.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var trackImage: UIImage? { get set }
```

## Discussion

If you provide a custom image, the trackTintColor property is ignored.

## See Also

### Configuring the progress bar

var progressViewStyle: UIProgressView.Style

The current graphical style of the progress view.

var progressTintColor: UIColor?

The color shown for the portion of the progress bar that’s filled.

var progressImage: UIImage?

An image to use for the portion of the progress bar that’s filled.

var trackTintColor: UIColor?

The color shown for the portion of the progress bar that isn’t filled.

