

- Local Authentication
- LAContext
-  interactionNotAllowed 

Instance Property

# interactionNotAllowed

A Boolean value indicating whether authentication can be interactive.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+watchOS 4.0+

``` source
var interactionNotAllowed: Bool { get set }
```

## See Also

### Evaluating access controls

func evaluateAccessControl(SecAccessControl, operation: LAAccessControlOperation, localizedReason: String, reply: (Bool, (any Error)?) -> Void)

Evaluates an access control for a given operation.

enum LAAccessControlOperation

Operations to be evaluated for access control.

