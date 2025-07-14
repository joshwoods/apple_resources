

- CryptoTokenKit
- TKSmartCardUserInteraction
-  interactionTimeout 

Instance Property

# interactionTimeout

The timeout, in seconds, after the first key stroke. If set to `0`, the reader-defined default timeout is used. `0` by default.

iOSiPadOSMac Catalyst 13.1+macOS 10.11+tvOSvisionOSwatchOS

``` source
var interactionTimeout: TimeInterval { get set }
```

## See Also

### Configuring Timeout

var initialTimeout: TimeInterval

The timeout, in seconds, for initial interaction. If set to `0`, the reader-defined default timeout is used. `0` by default.

