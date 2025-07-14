

- CryptoTokenKit
- TKSmartCard
-  send(ins:p1:p2:data:le:) 

Instance Method

# send(ins:p1:p2:data:le:)

Synchronously transmits an APDU command to the card and returns the response.

iOSiPadOSMac CatalystmacOS 10.12+tvOSvisionOSwatchOS

``` source
func send(
    ins: UInt8,
    p1: UInt8,
    p2: UInt8,
    data: Data? = nil,
    le: Int? = nil
) throws -> (sw: UInt16, response: Data)
```

## Parameters 

`ins`  

The instruction code.

`p1`  

The first parameter.

`p2`  

The second parameter.

`data`  

The data field of the APDU, or `nil` if no input data field should be present—for example, a `case1` or `case2` APDU.

The length of the data serves as `Lc` field of the APDU.

`le`  

The expected number of bytes to be returned, or nil if no output data are expected—for example, a `case1` or `case3` APDU. Pass `0` to accept as many bytes as the card provides.

## Return Value

A tuple containing the result code as contained in the first two bytes (`SW1SW2`) of the returned data, and the returned data excluding the first two bytes.

## See Also

### Transmitting Data

func send(ins: UInt8, p1: UInt8, p2: UInt8, data: Data?, le: Int?, reply: (Data?, UInt16, (any Error)?) -> Void)

Asynchronously transmits an APDU command to the card, returning the response in a completion handler.

func withSession&lt;T>(() throws -> T) throws -> T

Synchronously begins a session, executes the given closure, and ends the session.

