

- CloudKit
- CKRecordZoneSubscription
-  init(coder:) 

Initializer

# init(coder:)

Creates a zone-based subscription from a serialized instance.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 6.0+

``` source
init(coder aDecoder: NSCoder)
```

## Parameters 

`aDecoder`  

The coder for decoding the serialized record zone subscription.

## See Also

### Creating a Zone-Based Subscription

convenience init(zoneID: CKRecordZone.ID)

Creates a subscription for all records in the specified record zone.

Deprecated

convenience init(zoneID: CKRecordZone.ID, subscriptionID: CKSubscription.ID)

Creates a named subscription for all records in the specified record zone.

