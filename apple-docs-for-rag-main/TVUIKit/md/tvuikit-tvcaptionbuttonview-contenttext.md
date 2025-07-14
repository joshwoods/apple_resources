

- TVUIKit
- TVCaptionButtonView
-  contentText 

Instance Property

# contentText

The text displayed in the main content view.

tvOS 12.0+

``` source
@MainActor
var contentText: String? { get set }
```

## Discussion

The content text is displayed in the caption button and indicates the purpose of the caption button. The last instance of contentImage or contentText that was set in your app is displayed by the caption button view.

## See Also

### Configuring the Caption Button

var contentImage: UIImage?

The image displayed in the main content view.

var title: String?

The title for the caption button.

var subtitle: String?

The subtitle of the caption button.

