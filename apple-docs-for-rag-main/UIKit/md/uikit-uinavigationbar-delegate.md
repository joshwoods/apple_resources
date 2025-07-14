

- UIKit
- UINavigationBar
-  delegate 

Instance Property

# delegate

The navigation bar’s delegate object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var delegate: (any UINavigationBarDelegate)? { get set }
```

## Discussion

The delegate must conform to the UINavigationBarDelegate protocol. The default value is `nil`.

If the navigation bar was created by a navigation controller and is being managed by that object, you must not change the value of this property. A navigation controller acts as the delegate for the navigation bar it creates.

## See Also

### Responding to navigation bar changes

protocol UINavigationBarDelegate

Methods that a navigation bar calls before and after it modifies its stack of navigation items.

