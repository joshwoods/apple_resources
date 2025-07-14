

- AppKit
- NSTextView
-  registerForServices() 

Type Method

# registerForServices()

Registers send and return types for the Services facility.

macOS

``` source
@MainActor
class func registerForServices()
```

## Discussion

This method is invoked automatically when the first instance of a text view is created; you should never need to invoke it directly.

Subclasses of `NSTextView` that wish to add support for new service types should override registerForServices() to call `super` and then register their own new types.

