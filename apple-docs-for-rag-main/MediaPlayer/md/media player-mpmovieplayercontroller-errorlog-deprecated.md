

- Media Player
- MPMoviePlayerController
-  errorLog Deprecated

Instance Property

# errorLog

A snapshot of the playback failure error log for the movie player if it is playing a network stream.

iOS 4.3–9.0DeprecatediPadOS 4.3–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var errorLog: MPMovieErrorLog! { get }
```

Deprecated

Use AVFoundation.

## Discussion

Can be `nil`. For information about movie error logs, refer to MPMovieErrorLog.

## See Also

### Retrieving movie logs

var accessLog: MPMovieAccessLog!

A snapshot of the network playback log for the movie player if it is playing a network stream.

Deprecated

