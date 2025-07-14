

- CarPlay
- CPGridButton
-  titleVariants 

Instance Property

# titleVariants

An array of title variants for the button.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var titleVariants: [String] { get }
```

## Discussion

When the system displays the button, it selects the title that best fits the available screen space, so arrange the titles from most to least preferred when creating a grid button. Also, localize each title for display to the user, and be sure to include at least one title in the array.

## See Also

### Obtaining Grid Button Information

var image: UIImage

The image displayed on the button.

