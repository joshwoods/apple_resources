

- AVFoundation
- AVAssetReader
- AVAssetReader.Status
-  AVAssetReader.Status.failed 

Case

# AVAssetReader.Status.failed

The asset reader can no longer read samples from its asset because of an error.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
case failed
```

## Discussion

Query the asset reader’s error property to determine the reason for the failure.

## See Also

### Status Values

case unknown

The asset reader is in an unknown state.

case reading

The asset reader is successfully reading samples from its asset.

case completed

The asset reader completes reading all samples within its specified time range.

case cancelled

The asset reader can no longer read samples because you canceled reading.

