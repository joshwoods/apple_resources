

- UIKit
- UIMenuLeaf
-  sender 

Instance Property

# sender

The object on behalf of which to perform the menu element’s primary action.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
var sender: Any? { get }
```

**Required**

## Discussion

The system populates this property during the execution of the menu element’s action (its handler or selector).

## See Also

### Performing actions

func performWithSender(Any?, target: Any?)

Performs the element’s primary action.

**Required**

