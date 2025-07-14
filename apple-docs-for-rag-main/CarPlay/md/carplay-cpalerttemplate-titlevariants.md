

- CarPlay
- CPAlertTemplate
-  titleVariants 

Instance Property

# titleVariants

The array of title variants.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var titleVariants: [String] { get }
```

## Discussion

When the system displays the alert, it selects the title that best fits the available screen space, so arrange the titles from most to least preferred when creating an alert template. Also, localize each title for display to the user, and be sure to include at least one title in the array.

## See Also

### Getting the Alert Information

var actions: [CPAlertAction]

The array of actions available on the alert.

