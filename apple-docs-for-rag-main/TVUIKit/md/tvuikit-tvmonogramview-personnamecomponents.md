

- TVUIKit
- TVMonogramView
-  personNameComponents 

Instance Property

# personNameComponents

The names used to create a monogram image.

tvOS 12.0+

``` source
@MainActor
var personNameComponents: PersonNameComponents? { get set }
```

## Discussion

If no image is provided, the monogram object creates an image using the first initial of the givenName and familyName attributes contained in this property. The person’s name appears below the monogram image.

## See Also

### Configuring a Monogram

var image: UIImage?

The custom image for the monogram.

var title: String?

The title for the monogram.

var subtitle: String?

The subtitle for the monogram.

