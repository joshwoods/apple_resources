

- CarPlay
- CPNavigationAlert
-  updateTitleVariants(\_:subtitleVariants:) 

Instance Method

# updateTitleVariants(\_:subtitleVariants:)

Updates title and subtitle variants.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
func updateTitleVariants(
    _ newTitleVariants: [String],
    subtitleVariants newSubtitleVariants: [String]
)
```

## Parameters 

`newTitleVariants`  

An array of localized, displayable titles. The system selects the title that fits in the available display space.

`newSubtitleVariants`  

An array of localized, displayable subtitles. The system selects the title that fits in the available display space.

## Discussion

You can update the navigation alert with new title and subtitle variants before presenting the alert or after displaying it. Updating a dismissed alert has no effect.

## See Also

### Getting Titles

var titleVariants: [String]

An array of title strings.

var subtitleVariants: [String]

An array of subtitle strings.

