

- Swift
- AnyHashable
-  base 

Instance Property

# base

The value wrapped by this instance.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var base: Any { get }
```

## Discussion

The `base` property can be cast back to its original type using one of the type casting operators (`as?`, `as!`, or `as`).

```
let anyMessage = AnyHashable("Hello world!")
if let unwrappedMessage = anyMessage.base as? String {
    print(unwrappedMessage)
}
// Prints "Hello world!"
```

