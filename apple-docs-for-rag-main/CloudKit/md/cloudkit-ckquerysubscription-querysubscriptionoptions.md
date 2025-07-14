

- CloudKit
- CKQuerySubscription
-  querySubscriptionOptions 

Instance Property

# querySubscriptionOptions

Options that define the behavior of the subscription.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 6.0+

``` source
var querySubscriptionOptions: CKQuerySubscription.Options { get }
```

## Discussion

Set the value of this property at initialization time. When you configure a query-based subscription, use one of the following values:

- firesOnRecordCreation

- firesOnRecordUpdate

- firesOnRecordDeletion

If you don’t set an option, the system throws an invalidArgumentException.

## See Also

### Accessing the Subscription Search Parameters

var predicate: NSPredicate

The matching criteria to apply to records.

struct Options

Configuration options for a query subscription.

