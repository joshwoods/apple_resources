

- StoreKit
- EntitlementTaskState
-  value 

Instance Property

# value

The entitlement value if the task is successful.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var value: Value? { get }
```

## Discussion

This value is `nil` while the value is loading, or if it fails to load for any reason.

Use value as a convenience to access the entitlement value in code that doesn’t depend on the reason the value can’t be accessed if it fails to load.

## See Also

### Getting the transaction with the entitlement

var transaction: VerificationResult&lt;Transaction>?

The transaction value if the task is successful.

