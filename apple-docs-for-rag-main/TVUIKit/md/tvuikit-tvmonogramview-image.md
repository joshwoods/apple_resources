

- TVUIKit
- TVMonogramView
-  image 

Instance Property

# image

The custom image for the monogram.

tvOS 12.0+

``` source
@MainActor
var image: UIImage? { get set }
```

## Discussion

If you supply an image, the system uses this image instead of a generic image or an image created from the name components.

## See Also

### Configuring a Monogram

var personNameComponents: PersonNameComponents?

The names used to create a monogram image.

var title: String?

The title for the monogram.

var subtitle: String?

The subtitle for the monogram.

