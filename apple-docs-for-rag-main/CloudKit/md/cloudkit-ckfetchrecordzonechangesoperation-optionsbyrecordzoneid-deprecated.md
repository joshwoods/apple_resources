

- CloudKit
- CKFetchRecordZoneChangesOperation
-  optionsByRecordZoneID Deprecated

Instance Property

# optionsByRecordZoneID

Configuration options for each record zone that the operation retrieves.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–5.0Deprecated

``` source
var optionsByRecordZoneID: [CKRecordZone.ID : CKFetchRecordZoneChangesOperation.ZoneOptions]? { get set }
```

Deprecated

Use configurationsByRecordZoneID instead.

## Discussion

You can associate each record zone ID with options that define what CloudKit fetches for that record zone. See CKFetchRecordZoneChangesOperation.ZoneOptions for more information.

