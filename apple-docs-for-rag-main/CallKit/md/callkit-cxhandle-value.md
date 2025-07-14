

- CallKit
- CXHandle
-  value 

Instance Property

# value

The value of the handle.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
var value: String { get }
```

## Discussion

A handle’s value corresponds to its type. For example, a handle with type equal to CXHandle.HandleType.phoneNumber should have a value consisting of a sequence of digits.

## See Also

### Accessing Handle Attributes

var type: CXHandle.HandleType

The type of the handle.

