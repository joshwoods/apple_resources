

- CloudKit
-  Local Records 

API Collection

# Local Records

Manipulate records on-device and save changes to the server.

## Overview

CloudKit uses records and record zones to manage your app’s schema and the data it contains. You create these objects on the user’s device and save them to iCloud. After saving the objects, other devices can access and use them.

Use CKRecord to create a record, which must have a record ID. The record ID consists of the record’s name and the ID of the record zone to store it in. If you don’t provide a record zone ID, CloudKit stores the record in the default zone. Record IDs must be unique within the database that contains the record. Derive a record’s name from an object that guarantees uniqueness, such as a UUID. CloudKit assigns a unique record name if you don’t provide one. After you create a record, assign its keys and their values, and then save it to iCloud with CKModifyRecordsOperation. Use the same operation to delete records.

CloudKit stores records in record zones, which allow you to group specific types of records. For example, you might store a `Product` record type in one zone, and a `Customer` record type in another. Storing records in zones can make fetching them more efficient because you can scope queries, and other fetch operations, to a specific record zone to prevent searching the entire database. Only the private database supports custom record zones. Use CKRecordZone to create a zone, and then save it to the user’s private database with CKModifyRecordZonesOperation. The same operation supports deleting record zones. When you delete a zone, CloudKit deletes all the records it contains. To retrieve one or more record zones from iCloud, use CKFetchRecordZonesOperation. After you save a zone, create a record zone subscription. CloudKit uses subscriptions to notify your app of record changes. For more information, see Remote Records.

To allow users to share records, you must store those records in a custom record zone. For more information, see Shared Records.

CloudKit provides two ways to fetch records from iCloud. If you know the IDs of the records to fetch, use CKFetchRecordsOperation. Otherwise, use CKQuery and CKQueryOperation. A query consists of a record type, a predicate that defines criteria, and sort descriptors. You can further scope a query to retrieve records from a specific record zone. Queries limit the number of records they return. If the record count exceeds the limit, iCloud returns a subset of records and a cursor. You then use the cursor to fetch the next batch of records in another operation.

It’s important to consider the cost of a record when fetching it, especially when the record contains one or more assets. Both CKFetchRecordsOperation and CKQueryOperation provide a `desiredKeys` property, which allows you to specify the fields the operation retrieves from iCloud. If you don’t immediately need any associated assets, use `desiredKeys` to exclude the corresponding fields. You can then download individual assets as you need them.

The following example shows how to construct a query operation. It searches a specific record zone for properties in Cupertino, and uses a sort descriptor to request that iCloud returns the results in chronological order. The operation excludes a field that contains an asset using desiredKeys. For brevity, the example omits configuring the operation’s callbacks and executing it.

```
// Create a predicate that performs a case-insensitive search 
// of the record's address field for the value 'Cupertino'.
let predicate = NSPredicate(format: "address CONTAINS[c] 'Cupertino'")

// Use the predicate to create a query. Limit the query to 
// only retrieve records of the 'Property' record type.
let query = CKQuery(recordType: "Property", predicate: predicate)

// Set the query's sort descriptors so that iCloud returns 
// the records in chronological order.
query.sortDescriptors = [
    NSSortDescriptor(key: "creationDate", ascending: true)
]

// Use the query to create a query operation. Scope the 
// operation to the record zone that contains property
// records.
let operation = CKQueryOperation(query: query)
operation.zoneID = propertiesRecordZone.zoneID

// Each property has an address, a brochure, an owner, and
// a sale price. Don't include the 'brochure' field in the 
// query results. It contains a PDF asset, which can be 
// several megabytes in size.
operation.desiredKeys = [
    "address",
    "ownerName",
    "salePrice"
]
```

## Topics

### Transactions

class CKModifyRecordZonesOperation

An operation that modifies one or more record zones.

class CKModifyRecordsOperation

An operation that modifies one or more records.

### Fetch Requests

class CKFetchRecordZonesOperation

An operation for retrieving record zones from a database.

class CKFetchRecordsOperation

An operation for retrieving records from a database.

### Queries

class CKQuery

A query that describes the criteria to apply when searching for records in a database.

class CKQueryOperation

An operation for executing queries in a database.

class CKLocationSortDescriptor

An object for sorting records that contain location data.

### Base Objects

class CKDatabaseOperation

The abstract base class for operations that act upon databases in CloudKit.

## See Also

### Records

Remote Records

Use subscriptions and change tokens to efficiently manage modifications to remote records.

class CKSyncEngine

An object that manages the synchronization of local and remote record data.

Shared Records

Share one or more records with other iCloud users.

