

- CloudKit
- CKSyncEngine
-  cancelOperations() 

Instance Method

# cancelOperations()

Cancels any in-progress or pending sync operations.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
final func cancelOperations() async
```

## Discussion

The sync engine processes cancelation requests asynchronously, meaning it’s possible for in-progress operations to complete even after this method returns.

