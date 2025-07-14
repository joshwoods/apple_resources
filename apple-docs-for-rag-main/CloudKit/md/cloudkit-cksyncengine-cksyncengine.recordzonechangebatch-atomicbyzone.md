

- CloudKit
- CKSyncEngine
- CKSyncEngine.RecordZoneChangeBatch
-  atomicByZone 

Instance Property

# atomicByZone

A Boolean value that determines whether CloudKit modifies records atomically by record zone.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
var atomicByZone: Bool
```

## Discussion

When true, CloudKit processes record changes atomically by record zone, and if any individual change fails, all other changes in that record’s record zone fail and return an error of type CKError.Code.batchRequestFailed.

The default value is false.

