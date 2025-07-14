

- TVUIKit
- TVCaptionButtonView
-  contentImage 

Instance Property

# contentImage

The image displayed in the main content view.

tvOS 12.0+

``` source
@MainActor
var contentImage: UIImage? { get set }
```

## Discussion

The content image is displayed in the caption button and indicates the purpose of the caption button. The last instance of contentImage or contentText that was set in your app is displayed by the caption button view.

## See Also

### Configuring the Caption Button

var contentText: String?

The text displayed in the main content view.

var title: String?

The title for the caption button.

var subtitle: String?

The subtitle of the caption button.

