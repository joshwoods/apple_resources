

- CryptoTokenKit
- TKSmartCardATR
-  interfaceGroup(at:) 

Instance Method

# interfaceGroup(at:)

Returns the interface group at the specified index.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func interfaceGroup(at index: Int) -> TKSmartCardATR.InterfaceGroup?
```

## Parameters 

`index`  

The index of the desired interface group.

Important

Interface group indexes start at `1`, as specified by ISO 7816-3.

## Return Value

The interface group at the specified index, or `nil` if not present.

## See Also

### Retrieving Interface Groups

func interfaceGroup(for: TKSmartCardProtocol) -> TKSmartCardATR.InterfaceGroup?

Returns the interface group with the specified protocol.

class InterfaceGroup

A single interface-bytes group for a Smart Card ATR (Answer to Reset).

