

- AVFoundation
-  AVPlayerInterstitialEventAssetListResponseStatus 

Enumeration

# AVPlayerInterstitialEventAssetListResponseStatus

Constants that describe the status of the asset list response for an interstitial event.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
enum AVPlayerInterstitialEventAssetListResponseStatus
```

## Topics

### Status values

case available

Indicates that a valid asset list response is available.

case cleared

Indicates that the system cleared the asset list response.

case unavailable

Indicates that the asset list response is unavailable.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Monitoring the asset list response

class let assetListResponseStatusDidChangeNotification: NSNotification.Name

A notification the system posts when the status of an interstitial event’s asset list response changes.

