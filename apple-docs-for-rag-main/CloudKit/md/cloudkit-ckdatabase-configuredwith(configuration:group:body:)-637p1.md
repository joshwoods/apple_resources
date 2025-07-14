

- CloudKit
- CKDatabase
-  configuredWith(configuration:group:body:) 

Instance Method

# configuredWith(configuration:group:body:)

Applies a temporary configuration to the database within the scope of a closure that supports concurrency.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
@discardableResult @preconcurrency
func configuredWith(
    configuration: CKOperation.Configuration? = nil,
    group: CKOperationGroup? = nil,
    body: (CKDatabase) async throws -> R
) async rethrows -> R
```

## Parameters 

`configuration`  

An interim configuration to apply to the current database.

`group`  

The group to associate with the methods you execute in the closure. Specifying a group helps the system prioritize those method calls, and helps you identify the calls in the server logs in CloudKit Console. For more information, see CKOperationGroup.

`body`  

The closure to execute with the temporarily configured database.

## Discussion

Use this method to apply a specific configuration to the current database that lasts only for the duration of the trailing closure. For example, you might want to temporarily elevate the quality of service (QoS) for a group of method calls, or allow one or more expensive method calls to execute only while the device is using WiFi.

```
func fetchRecords(with ids: [CKRecord.ID]) async throws
    -> [CKRecord.ID: Result] {

    // Get a reference to the user's private database.
    let database = CKContainer.default().privateCloudDatabase

    // Create a configuration that denies cellular access.
    let config = CKOperation.Configuration()
    config.allowsCellularAccess = false

    // Configure the database and execute an expensive fetch.
    return try await database.configuredWith(configuration: config) { db in
        try await db.records(for: ids)
    }
}
```

## See Also

### Configuring Database Requests

func configuredWith&lt;R>(configuration: CKOperation.Configuration?, group: CKOperationGroup?, body: (CKDatabase) throws -> R) rethrows -> R

Applies a temporary configuration to the database within the scope of a closure.

