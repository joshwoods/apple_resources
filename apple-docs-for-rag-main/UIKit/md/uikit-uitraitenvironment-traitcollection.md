

- UIKit
- UITraitEnvironment
-  traitCollection 

Instance Property

# traitCollection

The traits, such as the size class and scale factor, that describe the current environment of the object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var traitCollection: UITraitCollection { get }
```

**Required**

## Mentioned in 

Displaying and managing views with a view controller

## Discussion

UIViewController and UIView adopt the UITraitEnvironment protocol and expose this property.

Important

Don’t implement this property in your own objects. Instead, use the traitCollection property associated with a view, view controller, or other object to determine the currently available trait information.

