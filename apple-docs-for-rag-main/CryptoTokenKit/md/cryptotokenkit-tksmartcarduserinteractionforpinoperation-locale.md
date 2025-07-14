

- CryptoTokenKit
- TKSmartCardUserInteractionForPINOperation
-  locale 

Instance Property

# locale

The locale for the displayed messages. If `nil`, the user’s current locale is used. By default, this value is the current locale of the system.

iOSiPadOSMac Catalyst 13.1+macOS 10.11+tvOSvisionOSwatchOS

``` source
var locale: Locale! { get set }
```

## See Also

### Configuring Messages

var pinMessageIndices: [NSNumber]?

A list of message indices referring to a predefined message table, used to specify the type and number of messages displayed during the PIN operation. `nil` by default.

