

- CloudKit
- CKFetchRecordZoneChangesOperation
-  CKFetchRecordZoneChangesOperation.ZoneOptions Deprecated

Class

# CKFetchRecordZoneChangesOperation.ZoneOptions

A configuration object that describes the information to fetch from a record zone.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–5.0Deprecated

``` source
class ZoneOptions
```

Deprecated

Use CKFetchRecordZoneChangesOperation.ZoneConfiguration instead.

## Topics

### Zone Change Options

var desiredKeys: [String]?

The fields to fetch for the requested records.

var previousServerChangeToken: CKServerChangeToken?

The token that identifies the starting point for retrieving changes.

var resultsLimit: Int

The maximum number of records to fetch from the record zone.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Deprecated Methods

convenience init(recordZoneIDs: [CKRecordZone.ID], optionsByRecordZoneID: [CKRecordZone.ID : CKFetchRecordZoneChangesOperation.ZoneOptions]?)

Creates an operation for fetching record zone changes.

Deprecated

