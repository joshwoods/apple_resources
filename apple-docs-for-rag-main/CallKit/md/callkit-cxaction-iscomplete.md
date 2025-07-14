

- CallKit
- CXAction
-  isComplete 

Instance Property

# isComplete

A Boolean value that indicates whether the action has been performed by the provider.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
var isComplete: Bool { get }
```

## Discussion

This property is initialized to false, and is set to true when either the fulfill() or fail() method is called.

## See also

### Related Documentation

- fulfill()

- fail()

## See Also

### Accessing Action Attributes

var uuid: UUID

The unique identifier for the action.

var timeoutDate: Date

The time after which the action cannot be completed.

