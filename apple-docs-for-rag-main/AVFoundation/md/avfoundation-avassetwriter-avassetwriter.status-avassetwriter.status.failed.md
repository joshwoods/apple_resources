

- AVFoundation
- AVAssetWriter
- AVAssetWriter.Status
-  AVAssetWriter.Status.failed 

Case

# AVAssetWriter.Status.failed

The asset writer fails to write the output file.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
case failed
```

## Discussion

Query the error property value to determine the cause of the failure.

## See Also

### Status Values

case unknown

The asset writer’s status isn’t known.

case writing

The asset writer is writing.

case completed

The asset writer finishes writing successfully.

case cancelled

The asset writer canceled the writing operation.

