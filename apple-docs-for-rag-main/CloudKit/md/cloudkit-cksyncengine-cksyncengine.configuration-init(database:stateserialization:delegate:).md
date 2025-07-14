

- CloudKit
- CKSyncEngine
- CKSyncEngine.Configuration
-  init(database:stateSerialization:delegate:) 

Initializer

# init(database:stateSerialization:delegate:)

Creates a configuration for the specified database and serialized state.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
init(
    database: CKDatabase,
    stateSerialization: CKSyncEngine.State.Serialization?,
    delegate: any CKSyncEngineDelegate
)
```

## Parameters 

`database`  

The database to sync — either a person’s private database or their shared database.

`stateSerialization`  

If this is the first initialization of the associated sync engine, specify `nil`; otherwise, specify the state from the most recent CKSyncEngine.Event.stateUpdate(_:) event that your delegate handled.

`delegate`  

The object that provides the records to sync and handles any related events.

