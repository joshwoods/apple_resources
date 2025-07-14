

- AVFoundation
- AVPlayerInterstitialEventMonitor
-  assetListResponseStatusDidChangeNotification 

Type Property

# assetListResponseStatusDidChangeNotification

A notification the system posts when the status of an interstitial event’s asset list response changes.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
class let assetListResponseStatusDidChangeNotification: NSNotification.Name
```

## Discussion

Notifications of this type provide a userInfo dictionary that can contain values for the keys listed below.

## Topics

### User information keys

let AVPlayerInterstitialEventMonitorAssetListResponseStatusDidChangeEventKey: String

A key to retrieve the interstitial event that has an asset list response status change.

let AVPlayerInterstitialEventMonitorAssetListResponseStatusDidChangeStatusKey: String

A key to retrieve the asset list response status.

let AVPlayerInterstitialEventMonitorAssetListResponseStatusDidChangeErrorKey: String

A key to retrieve the error related to a change in an interstitial event’s asset list response.

## See Also

### Monitoring the asset list response

enum AVPlayerInterstitialEventAssetListResponseStatus

Constants that describe the status of the asset list response for an interstitial event.

