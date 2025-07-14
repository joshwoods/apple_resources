

- UIKit
- UITabBar
-  endCustomizing(animated:) 

Instance Method

# endCustomizing(animated:)

Dismisses the standard interface used to customize the tab bar.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+

``` source
@MainActor
func endCustomizing(animated: Bool) -> Bool
```

## Parameters 

`animated`  

If true, animate the dismissal of the interface.

## Return Value

true if items on the tab bar changed or false if they did not.

## Discussion

You rarely need to call this method. Typically, the user dismisses the modal view by tapping the built-in Done button in the interface. However, you might call this method to cancel the customization process because of changes to other parts of your interface.

## See Also

### Supporting user customization of tab bars

func beginCustomizingItems([UITabBarItem])

Presents a standard interface that lets the user customize the contents of the tab bar.

var isCustomizing: Bool

A Boolean value indicating whether the user is currently customizing the tab bar.

