

- UIKit
- UIProgressView
-  progressViewStyle 

Instance Property

# progressViewStyle

The current graphical style of the progress view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var progressViewStyle: UIProgressView.Style { get set }
```

## Discussion

The value of this property is a constant that specifies the style of the progress view. The default style is UIProgressView.Style.default. For more on these constants, see UIProgressView.Style.

## See Also

### Configuring the progress bar

var progressTintColor: UIColor?

The color shown for the portion of the progress bar that’s filled.

var progressImage: UIImage?

An image to use for the portion of the progress bar that’s filled.

var trackTintColor: UIColor?

The color shown for the portion of the progress bar that isn’t filled.

var trackImage: UIImage?

An image to use for the portion of the track that isn’t filled.

