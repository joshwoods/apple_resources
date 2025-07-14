

- UIKit
- UIDeferredMenuElement
-  uncached(\_:) 

Type Method

# uncached(\_:)

Returns a placeholder menu element that the system replaces with the result of the provider’s completion handler.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
class func uncached(_ elementProvider: @escaping (@escaping ([UIMenuElement]) -> Void) -> Void) -> Self
```

## Parameters 

`elementProvider`  

The closure the system calls to request the deferred menu items.

## Discussion

When you use this initializer, the system calls each deferred element’s completion closure every time it encounters the element in a menu. The system doesn’t cache the element for reuse.

## See Also

### Creating a deferred menu element

convenience init((([UIMenuElement]) -> Void) -> Void)

A convenience initializer that creates a placeholder menu element that the system replaces with the result of the provider’s completion handler.

