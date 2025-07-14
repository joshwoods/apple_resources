

- CloudKit
- CKSyncEngine
- CKSyncEngine.Configuration
-  delegate 

Instance Property

# delegate

The object that provides the records to sync and handles any related events.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
var delegate: any CKSyncEngineDelegate
```

## See Also

### Handling record changes

protocol CKSyncEngineDelegate

An interface for providing record data to a sync engine and customizing that engine’s behavior.

