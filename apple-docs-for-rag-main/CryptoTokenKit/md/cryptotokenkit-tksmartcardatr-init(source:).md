

- CryptoTokenKit
- TKSmartCardATR
-  init(source:) 

Initializer

# init(source:)

Initializes a `TKSmartCardATR` object from a provided data source.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
init?(source: @escaping () -> Int32)
```

## Parameters 

`source`  

The block providing a stream of data for an ATR.

The block takes no arguments and returns one byte. To indicate that an error occured, the block returns `-1`.

## Return Value

A `TKSmartCardATR` object initialized with the parsed data. If the byte stream produces an error or does not contain a valid ATR, returns `nil`.

## See Also

### Creating a Smart Card ATR

init?(bytes: Data)

Initializes a `TKSmartCardATR` object from a provided data object.

