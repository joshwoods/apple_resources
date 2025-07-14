

- SwiftUI
- EnvironmentValues
-  menuIndicatorVisibility 

Instance Property

# menuIndicatorVisibility

The menu indicator visibility to apply to controls within a view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var menuIndicatorVisibility: Visibility { get set }
```

## Discussion

Note

On tvOS, the standard button styles do not include a menu indicator, so this modifier will have no effect when using a built-in button style. You can implement an indicator in your own ButtonStyle implementation by checking the value of this environment value.

## See Also

### Showing a menu indicator

func menuIndicator(Visibility) -> some View

Sets the menu indicator visibility for controls within this view.

