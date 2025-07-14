

- TVUIKit
- TVPosterView
-  image 

Instance Property

# image

The image for the poster view.

tvOS 12.0+

``` source
@MainActor
var image: UIImage? { get set }
```

## Discussion

The size of the poster view is determined by the natural size of the supplied image when no frame or content size is explicitly set.

## See Also

### Configuring a Poster View

var imageView: UIImageView

The image view associated with the poster view.

var title: String?

The title for the poster view.

var subtitle: String?

The subtitle for the poster view.

