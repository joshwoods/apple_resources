

- SceneKit
- SCNTransaction
-  completionBlock 

Type Property

# completionBlock

Returns the block previously associated with the current transaction.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class var completionBlock: (() -> Void)? { get set }
```

## Discussion

See `setCompletionBlock(_:)`, `setCompletionBlock:` in Objective-C, for a description of the role of the completion block object.

