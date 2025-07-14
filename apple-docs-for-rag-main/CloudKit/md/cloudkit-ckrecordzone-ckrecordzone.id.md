

- CloudKit
- CKRecordZone
-  CKRecordZone.ID 

Class

# CKRecordZone.ID

An object that uniquely identifies a record zone in a database.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
class ID
```

## Overview

Zones are a mechanism for grouping related records together. You create zone ID objects when you want to fetch an existing zone object or create a new zone with a specific name.

A record zone ID distinguishes one zone from another by a name string and the ID of the user who creates the zone. Both strings must be ASCII strings that don’t exceed 255 characters. When creating your own record zone ID objects, you can use names that have more meaning to your app or to the user, providing each zone name is unique within the specified database. The owner name must be either the current user name or the name of another user. Get the current user name from CKCurrentUserDefaultName or by calling fetchUserRecordID(completionHandler:).

When creating new record zones, make the name string in the record zone ID unique in the target database. Public databases don’t support custom zones, and only the user who owns the database can create zones in private databases.

Don’t create subclasses of this class.

### Interacting with Record Zone IDs

After you create a record zone ID, interactions with it typically include:

- Creating a CKRecord.ID object so that you can fetch or create records in that zone.

- Retrieving an existing CKRecordZone object from the database.

You don’t need to create a record zone ID to create a record zone. The CKRecordZone class has initialization methods that create a record zone ID using the name string you provide.

#### Creating Record Zone IDs for Records

To create a new record in a custom zone, create a record zone ID that specifies the zone name. Use the record zone ID to create a CKRecord.ID, and then use the record ID to create the record.

#### Fetching a Record Zone Object from the Database

To fetch a record zone from the database, use a CKFetchRecordZonesOperation object or the fetch(withRecordZoneID:completionHandler:) method of CKDatabase. Both techniques accept a record zone ID that you provide and retrieve the corresponding record zone object asynchronously. If you use the operation object, you can retrieve multiple record zones at the same time.

## Topics

### Creating a Record Zone ID

convenience init(zoneName: String, ownerName: String)

Creates a record zone ID with the specified name and owner.

### Getting the Record Zone ID Attributes

var zoneName: String

The unique name of the record zone.

var ownerName: String

The ID of the user who owns the record zone.

### Accessing the Default Zone

static let `default`: CKRecordZone.ID

The default zone ID.

static let defaultZoneName: String

The name of the default zone.

### Initializers

convenience init(zoneName: String, ownerName: String?)Deprecated

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

### Creating a Record Zone

init(zoneName: String)

Creates a record zone object with the specified zone name.

init(zoneID: CKRecordZone.ID)

Creates a record zone object with the specified zone ID.

