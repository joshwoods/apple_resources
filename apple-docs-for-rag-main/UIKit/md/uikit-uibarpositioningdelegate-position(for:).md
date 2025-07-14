

- UIKit
- UIBarPositioningDelegate
-  position(for:) 

Instance Method

# position(for:)

Asks the delegate for the position of the specified bar in its new window.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func position(for bar: any UIBarPositioning) -> UIBarPosition
```

## Parameters 

`bar`  

The bar that was added to the window.

## Return Value

The position of the bar.

## Discussion

If your interface has a custom bar with a delegate, that delegate can implement this method and use it to specify the position of the bar that has been added to a window.

Delegates for the UINavigationBar and UISearchBar classes return the value UIBarPosition.top by default. The delegate of the UIToolbar class returns the value UIBarPosition.bottom by default.

## See Also

### Related Documentation

protocol UIBarPositioning

A set of methods for defining the positioning of bars in iOS apps.

