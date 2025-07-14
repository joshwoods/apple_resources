

- CloudKit
- CKRecordZoneSubscription
-  init(zoneID:) Deprecated

Initializer

# init(zoneID:)

Creates a subscription for all records in the specified record zone.

iOS 10.0–10.0DeprecatediPadOS 10.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.12DeprecatedtvOS 10.0–10.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 6.0–6.0Deprecated

``` source
convenience init(zoneID: CKRecordZone.ID)
```

## Parameters 

`zoneID`  

The ID of the record zone that contains the records you want to monitor. This parameter must not be `nil`.

## Discussion

The subscription that this method returns is a zone-based subscription that generates push notifications when CloudKit changes any of the specificed record zone’s records.

## See Also

### Creating a Zone-Based Subscription

convenience init(zoneID: CKRecordZone.ID, subscriptionID: CKSubscription.ID)

Creates a named subscription for all records in the specified record zone.

init(coder: NSCoder)

Creates a zone-based subscription from a serialized instance.

