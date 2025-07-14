

- CarPlay
- CPDashboardButton
-  init(titleVariants:subtitleVariants:image:handler:) 

Initializer

# init(titleVariants:subtitleVariants:image:handler:)

Creates a dashboard button that displays a title, an optional subtitle, and an image.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
init(
    titleVariants: [String],
    subtitleVariants: [String],
    image: UIImage,
    handler: ((CPDashboardButton) -> Void)? = nil
)
```

## Parameters 

`titleVariants`  

An array of string variants to use for the button’s title.

`subtitleVariants`  

An array of string variants to use for the button’s subtitle.

`image`  

The image to display on the button.

`handler`  

The block that CarPlay invokes when the user taps the button.

## Return Value

A button that displays the provided title, subtitle, and image.

## Discussion

You must provide at least one, nonzero length title variant, and an image for the button to display. CarPlay displays the first variant that fits into the available screen space, so arrange your title and subtitle variant arrays from most- to least-preferred. Provide the variant strings as localized, displayable content.

The maximum supported image size is 30 x 30 points.

