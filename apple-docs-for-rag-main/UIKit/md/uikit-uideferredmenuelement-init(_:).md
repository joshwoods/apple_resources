

- UIKit
- UIDeferredMenuElement
-  init(\_:) 

Initializer

# init(\_:)

A convenience initializer that creates a placeholder menu element that the system replaces with the result of the provider’s completion handler.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
convenience init(_ elementProvider: @escaping (@escaping ([UIMenuElement]) -> Void) -> Void)
```

## Parameters 

`elementProvider`  

The closure the system calls to request the deferred menu items.

## Discussion

The system calls each element’s closure once, when it first encounters the element in a menu. Once provided, the system caches the element and may reuse it across menus.

You can use uncached(_:) to initialize a deferred menu element without caching. With caching disabled, the system calls the provider closure each time it displays the element.

## See Also

### Creating a deferred menu element

class func uncached((([UIMenuElement]) -> Void) -> Void) -> Self

Returns a placeholder menu element that the system replaces with the result of the provider’s completion handler.

