

- CloudKit
- CKQuerySubscription
-  recordType 

Instance Property

# recordType

The type of record that the subscription queries.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOSwatchOS 6.0+Swift 4.2+

``` source
var recordType: CKRecord.RecordType? { get }
```

## Discussion

This property only applies to query-based subscriptions. CloudKit sets its value when you create the subscription. For all other types of subscription, CloudKit ignores this property and sets its value to `nil`.

## See Also

### Accessing the Subscription Metadata

var zoneID: CKRecordZone.ID?

The ID of the record zone that the subscription queries.

