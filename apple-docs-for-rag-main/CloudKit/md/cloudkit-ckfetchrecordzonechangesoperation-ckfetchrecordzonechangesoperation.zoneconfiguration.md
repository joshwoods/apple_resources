

- CloudKit
- CKFetchRecordZoneChangesOperation
-  CKFetchRecordZoneChangesOperation.ZoneConfiguration 

Class

# CKFetchRecordZoneChangesOperation.ZoneConfiguration

A configuration object that describes the information to fetch from a record zone.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class ZoneConfiguration
```

## Topics

### Creating a Zone Change Configuration

convenience init(previousServerChangeToken: CKServerChangeToken?, resultsLimit: Int?, desiredKeys: [CKRecord.FieldKey]?)

Creates a zone configuration with the desired keys and a result limit for updates.

### Accessing a Zone Change Configuration

var previousServerChangeToken: CKServerChangeToken?

The server change token.

var resultsLimit: Int

The maximum number of records that CloudKit retrieves when fetching zone changes.

var desiredKeys: [CKRecord.FieldKey]?

An array of the record keys to retrieve.

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
- Sendable

## See Also

### Configuring the Zone Change Operation

var configurationsByRecordZoneID: [CKRecordZone.ID : CKFetchRecordZoneChangesOperation.ZoneConfiguration]?

A dictionary of configurations for fetching change operations by zone identifier.

var fetchAllChanges: Bool

A Boolean value that indicates whether to send repeated requests to the server.

var recordZoneIDs: [CKRecordZone.ID]?

The IDs of the record zones that contain the records to fetch.

