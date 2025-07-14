

- TVUIKit
- TVPosterView
-  init(image:) 

Initializer

# init(image:)

Creates a new poster view using the supplied image.

tvOS 12.0+

``` source
@MainActor
init(image: UIImage?)
```

## Parameters 

`image`  

The image to be displayed in the content view area of the lockup view.

## Discussion

The size of the poster view is determined by the natural size of the passed image when no frame or content size is explicitly set.

