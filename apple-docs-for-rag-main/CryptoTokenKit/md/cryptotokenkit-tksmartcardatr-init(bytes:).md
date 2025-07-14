

- CryptoTokenKit
- TKSmartCardATR
-  init(bytes:) 

Initializer

# init(bytes:)

Initializes a `TKSmartCardATR` object from a provided data object.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
init?(bytes: Data)
```

## Parameters 

`bytes`  

The ATR data to be parsed.

## Return Value

A `TKSmartCardATR` object initialized with the parsed data. If `bytes` does not contain a valid ATR, returns `nil`.

## See Also

### Creating a Smart Card ATR

init?(source: () -> Int32)

Initializes a `TKSmartCardATR` object from a provided data source.

