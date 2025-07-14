

- UIKit
- UIViewController
-  extensionContext 

Instance Property

# extensionContext

Returns the extension context of the view controller.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var extensionContext: NSExtensionContext? { get }
```

## Discussion

The view controller can check this property to see if it participates in an extension request. If no extension context is set for the current view controller, the system walks up the view controller hierarchy to find a parent view controller that has a non `nil` `extensionContext` value.

