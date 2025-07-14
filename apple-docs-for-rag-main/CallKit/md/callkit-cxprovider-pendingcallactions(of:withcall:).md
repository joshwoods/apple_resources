

- CallKit
- CXProvider
-  pendingCallActions(of:withCall:) 

Instance Method

# pendingCallActions(of:withCall:)

Returns all call actions in any pending transactions of the specified class for the specified call identifier that are incomplete.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
func pendingCallActions(
    of callActionClass: AnyClass,
    withCall callUUID: UUID
) -> [CXCallAction]
```

## Parameters 

`callActionClass`  

The desired CXCallAction subclass of returned actions.

`callUUID`  

The desired call identifier for returned actions.

## Return Value

An array of call actions of the specified class for the specified call identifier.

## See Also

### Accessing Pending Transaction and Call Actions

var pendingTransactions: [CXTransaction]

Incomplete transactions.

