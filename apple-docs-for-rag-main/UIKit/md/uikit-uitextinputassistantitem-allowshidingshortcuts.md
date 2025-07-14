

- UIKit
- UITextInputAssistantItem
-  allowsHidingShortcuts 

Instance Property

# allowsHidingShortcuts

A Boolean value that indicates whether the user can hide the shortcuts bar.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+

``` source
@MainActor
var allowsHidingShortcuts: Bool { get set }
```

## Discussion

When the value of this property is true, the user may hide the shortcuts bar when the keyboard is visible. When the value is false, the shortcuts bar remains visible while the keyboard is visible. The default value of this property is true.

## See Also

### Configuring the shortcuts bar

var leadingBarButtonGroups: [UIBarButtonItemGroup]

The array of button item groups to display before the typing suggestions.

var trailingBarButtonGroups: [UIBarButtonItemGroup]

The array of button item groups to display after the typing suggestions.

