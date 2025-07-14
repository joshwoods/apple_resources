

- Network Extension
- NWUDPSession
-  writeDatagram(\_:completionHandler:) Deprecated

Instance Method

# writeDatagram(\_:completionHandler:)

Write a single datagram.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func writeDatagram(
    _ datagram: Data,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

Deprecated

Use the nw_connection_send(_:_:_:_:_:) function from the Network framework instead.

## Parameters 

`datagram`  

An NSData object containing the datagram to write. To improve performance, this should be an immutable data object.

`completionHandler`  

A handler called when the write request has either succeeded or failed.

## Discussion

Callers should wait until the `completionHandler` is executed before issuing another write.

## See Also

### Transferring data

func setReadHandler(([Data]?, (any Error)?) -> Void, maxDatagrams: Int)

Set a read handler for datagrams.

Deprecated

func writeMultipleDatagrams([Data], completionHandler: ((any Error)?) -> Void)

Write multiple datagrams.

Deprecated

var maximumDatagramLength: Int

The maximum size of a datagram to be written currently.

Deprecated

