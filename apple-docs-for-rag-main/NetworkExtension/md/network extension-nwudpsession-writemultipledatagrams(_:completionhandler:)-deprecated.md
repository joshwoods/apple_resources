

- Network Extension
- NWUDPSession
-  writeMultipleDatagrams(\_:completionHandler:) Deprecated

Instance Method

# writeMultipleDatagrams(\_:completionHandler:)

Write multiple datagrams.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func writeMultipleDatagrams(
    _ datagramArray: [Data],
    completionHandler: @escaping ((any Error)?) -> Void
)
```

Deprecated

Use the nw_connection_send(_:_:_:_:_:) function from the Network framework instead.

## Parameters 

`datagramArray`  

An NSArray of NSData objects, containing the ordered list of datagrams to write.

`completionHandler`  

A handler called when the write request has either succeeded or failed.

## Discussion

Callers should wait until the `completionHandler` is executed before issuing another write.

## See Also

### Transferring data

func setReadHandler(([Data]?, (any Error)?) -> Void, maxDatagrams: Int)

Set a read handler for datagrams.

Deprecated

func writeDatagram(Data, completionHandler: ((any Error)?) -> Void)

Write a single datagram.

Deprecated

var maximumDatagramLength: Int

The maximum size of a datagram to be written currently.

Deprecated

