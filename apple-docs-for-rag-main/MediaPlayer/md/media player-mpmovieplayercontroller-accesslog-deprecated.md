

- Media Player
- MPMoviePlayerController
-  accessLog Deprecated

Instance Property

# accessLog

A snapshot of the network playback log for the movie player if it is playing a network stream.

iOS 4.3–9.0DeprecatediPadOS 4.3–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var accessLog: MPMovieAccessLog! { get }
```

Deprecated

Use AVFoundation.

## Discussion

Can be `nil`. For information about movie access logs, refer to MPMovieAccessLog.

## See Also

### Retrieving movie logs

var errorLog: MPMovieErrorLog!

A snapshot of the playback failure error log for the movie player if it is playing a network stream.

Deprecated

