

- CarPlay
- CPNavigationAlert
-  titleVariants 

Instance Property

# titleVariants

An array of title strings.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var titleVariants: [String] { get }
```

## Discussion

Each title should be localized and ready for display to the user. The system selects the title to display based on the available screen space.

## See Also

### Getting Titles

var subtitleVariants: [String]

An array of subtitle strings.

func updateTitleVariants([String], subtitleVariants: [String])

Updates title and subtitle variants.

