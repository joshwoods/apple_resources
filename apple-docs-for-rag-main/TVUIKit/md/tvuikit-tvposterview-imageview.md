

- TVUIKit
- TVPosterView
-  imageView 

Instance Property

# imageView

The image view associated with the poster view.

tvOS 12.0+

``` source
@MainActor
var imageView: UIImageView { get }
```

## Discussion

Use the image view to add additional information, such as overlays or badges, to the main content image. Don’t set an image directly on the image view. Always use the poster view’s image property.

## See Also

### Configuring a Poster View

var image: UIImage?

The image for the poster view.

var title: String?

The title for the poster view.

var subtitle: String?

The subtitle for the poster view.

