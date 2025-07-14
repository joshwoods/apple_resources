

- AVFoundation
- AVAssetExportSession
-  maxDuration Deprecated

Instance Property

# maxDuration

Provides an estimate of the maximum duration of the exported media.

iOS 4.0–18.0DeprecatediPadOS 4.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.14–15.0DeprecatedtvOS 9.0–18.0Deprecated

``` source
var maxDuration: CMTime { get }
```

Deprecated

Use estimateMaximumDurationWithCompletionHandler: instead

## See Also

### Estimating Duration

func estimateMaximumDuration(completionHandler: (CMTime, (any Error)?) -> Void)

Starts estimating the maximum duration of the export while considering the asset, preset, and time range configuration of the export session.

