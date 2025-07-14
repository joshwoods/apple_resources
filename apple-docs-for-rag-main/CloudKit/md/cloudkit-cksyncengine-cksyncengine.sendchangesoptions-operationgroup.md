

- CloudKit
- CKSyncEngine
- CKSyncEngine.SendChangesOptions
-  operationGroup 

Instance Property

# operationGroup

The operation group to use for the underlying CloudKit operations.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
var operationGroup: CKOperationGroup { get set }
```

## Discussion

Tip

Providing a specific operation group helps you to identify and analyze the telemetry of send operations in CloudKit Console.

The default value is `nil`.

