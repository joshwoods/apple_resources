

- AVFoundation
- AVAssetReader
- AVAssetReader.Status
-  AVAssetReader.Status.cancelled 

Case

# AVAssetReader.Status.cancelled

The asset reader can no longer read samples because you canceled reading.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
case cancelled
```

## See Also

### Status Values

case unknown

The asset reader is in an unknown state.

case reading

The asset reader is successfully reading samples from its asset.

case completed

The asset reader completes reading all samples within its specified time range.

case failed

The asset reader can no longer read samples from its asset because of an error.

