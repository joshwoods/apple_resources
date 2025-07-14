

- CloudKit
-  Responding to Requests to Delete Data 

Article

# Responding to Requests to Delete Data

Provide options for users to delete their CloudKit data from your app.

## Overview

If your app stores data in CloudKit on behalf of your users, give them a simple way to delete their data.

### Identify Containers

To be sure that you delete all of a user’s data that your app stores in CloudKit, cross-reference the list of containers your app has access to in Xcode and assemble a list of those containers’ identifiers. Identifying an App’s Containers describes this process.

The example below stores containers in an array to use later for enumeration:

```
let containers: [CKContainer] = [
    CKContainer.default(),
    .init(identifier: "iCloud.com.example.myexampleapp.documents"),
    .init(identifier: "iCloud.com.example.myexampleapp.settings")
]
```

### Delete Records

The example below uses an instance of CKModifyRecordZonesOperation to delete all records in each container’s private database:

```
for container in containers {
    container.privateCloudDatabase.fetchAllRecordZones { zones, error in
        guard let zones = zones, error == nil else {
            print("Error fetching zones.")
            return
        }

        let zoneIDs = zones.map { $0.zoneID }
        let deletionOperation = CKModifyRecordZonesOperation(recordZonesToSave: nil, recordZoneIDsToDelete: zoneIDs)

        deletionOperation.modifyRecordZonesCompletionBlock = { _, deletedZones, error in
            guard error == nil else {
                let error = error!

                print("Error deleting records.", error)
                return
            }

            print("Records successfully deleted in this zone.")
        }

        container.privateCloudDatabase.add(deletionOperation)
    }
}
```

## See Also

### Privacy

Encrypting User Data

Deploy industry-standard security technologies using CloudKit encryption.

Providing User Access to CloudKit Data

Provide users access to the data your app stores on their behalf.

Changing Access Controls on User Data

Restrict access to or remove restrictions from a user’s data at their request.

class CKFetchWebAuthTokenOperation

An operation that creates an authentication token for use with CloudKit web services.

Identifying an App’s Containers

Use Xcode’s Project navigator to find the identifiers of active CloudKit containers.

