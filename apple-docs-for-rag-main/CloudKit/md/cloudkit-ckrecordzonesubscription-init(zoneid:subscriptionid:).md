

- CloudKit
- CKRecordZoneSubscription
-  init(zoneID:subscriptionID:) 

Initializer

# init(zoneID:subscriptionID:)

Creates a named subscription for all records in the specified record zone.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOSwatchOS 6.0+Swift 4.2+

``` source
convenience init(
    zoneID: CKRecordZone.ID,
    subscriptionID: CKSubscription.ID
)
```

## Parameters 

`zoneID`  

The ID of the record zone that contains the records you want to monitor.

`subscriptionID`  

The subscription’s name. It must be unique in the container and must not be an empty string.

## Discussion

The subscription that this method returns is a zone-based subscription that generates push notifications when CloudKit changes any of the specificed record zone’s records.

## See Also

### Creating a Zone-Based Subscription

convenience init(zoneID: CKRecordZone.ID)

Creates a subscription for all records in the specified record zone.

Deprecated

init(coder: NSCoder)

Creates a zone-based subscription from a serialized instance.

