

- AVFoundation
- AVAssetReader
- AVAssetReader.Status
-  AVAssetReader.Status.reading 

Case

# AVAssetReader.Status.reading

The asset reader is successfully reading samples from its asset.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
case reading
```

## See Also

### Status Values

case unknown

The asset reader is in an unknown state.

case completed

The asset reader completes reading all samples within its specified time range.

case failed

The asset reader can no longer read samples from its asset because of an error.

case cancelled

The asset reader can no longer read samples because you canceled reading.

