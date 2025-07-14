

- CloudKit
- CKQuerySubscription
-  predicate 

Instance Property

# predicate

The matching criteria to apply to records.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 6.0+

``` source
@NSCopying
var predicate: NSPredicate { get }
```

## Discussion

A query-based subscription uses its search predicate to identify potential matches for records. It combines the predicate information with the value in the querySubscriptionOptions property to determine when to send a push notification to the app.

The search predicate defines the records that the subscription object monitors for changes. The system only uses the property’s value when the subscriptionType property is CKSubscription.SubscriptionType.query. Otherwise, the system ignores it.

## See Also

### Accessing the Subscription Search Parameters

var querySubscriptionOptions: CKQuerySubscription.Options

Options that define the behavior of the subscription.

struct Options

Configuration options for a query subscription.

