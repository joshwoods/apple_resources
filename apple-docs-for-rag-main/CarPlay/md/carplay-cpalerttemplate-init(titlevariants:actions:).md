

- CarPlay
- CPAlertTemplate
-  init(titleVariants:actions:) 

Initializer

# init(titleVariants:actions:)

Creates an alert template.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
init(
    titleVariants: [String],
    actions: [CPAlertAction]
)
```

## Parameters 

`titleVariants`  

An array of title variants. Each title should be localized and ready for display to the user. When the system displays the alert, it selects the title that best fits the available screen space, so arrange the variants from most to least preferred. Always include at least one title in the array.

`actions`  

An array of actions available on the alert. The array must contain at least one action.

## Return Value

A newly initialized alert template.

## See Also

### Creating an Alert Template

class var maximumActionCount: Int

The maximum number of actions allowed in an alert template.

