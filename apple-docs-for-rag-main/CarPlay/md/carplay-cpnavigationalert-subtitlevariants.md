

- CarPlay
- CPNavigationAlert
-  subtitleVariants 

Instance Property

# subtitleVariants

An array of subtitle strings.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var subtitleVariants: [String] { get }
```

## Discussion

Each subtitle should be localized and ready for display to the user. The system selects the subtitle to display based on the available screen space.

## See Also

### Getting Titles

var titleVariants: [String]

An array of title strings.

func updateTitleVariants([String], subtitleVariants: [String])

Updates title and subtitle variants.

