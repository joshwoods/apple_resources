

- CloudKit
- CKFetchRecordZoneChangesOperation
-  init(recordZoneIDs:optionsByRecordZoneID:) Deprecated

Initializer

# init(recordZoneIDs:optionsByRecordZoneID:)

Creates an operation for fetching record zone changes.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–5.0Deprecated

``` source
convenience init(
    recordZoneIDs: [CKRecordZone.ID],
    optionsByRecordZoneID: [CKRecordZone.ID : CKFetchRecordZoneChangesOperation.ZoneOptions]? = nil
)
```

Deprecated

Use init(recordZoneIDs:configurationsByRecordZoneID:) instead.

## Parameters 

`recordZoneIDs`  

The IDs of the record zones that you want to query for changes.

`optionsByRecordZoneID`  

A dictionary that maps record zone IDs to their corresponding options. You can specify `nil` for this parameter.

## Discussion

CloudKit configures the operation for retrieving all of the record zones that you specify. If you want to reduce the amount of data that CloudKit returns, provide zone options for each record zone.

## See Also

### Deprecated Methods

class ZoneOptions

A configuration object that describes the information to fetch from a record zone.

Deprecated

