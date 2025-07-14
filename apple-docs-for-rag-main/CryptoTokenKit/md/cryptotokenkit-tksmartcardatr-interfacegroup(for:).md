

- CryptoTokenKit
- TKSmartCardATR
-  interfaceGroup(for:) 

Instance Method

# interfaceGroup(for:)

Returns the interface group with the specified protocol.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func interfaceGroup(for protocol: TKSmartCardProtocol) -> TKSmartCardATR.InterfaceGroup?
```

## Parameters 

`protocol`  

The protocol used by the desired interface group.

## Return Value

The interface group with the specified protocol, or `nil` if none exists.

## See Also

### Retrieving Interface Groups

func interfaceGroup(at: Int) -> TKSmartCardATR.InterfaceGroup?

Returns the interface group at the specified index.

class InterfaceGroup

A single interface-bytes group for a Smart Card ATR (Answer to Reset).

