

- Network Extension
- NWUDPSession
-  setReadHandler(\_:maxDatagrams:) Deprecated

Instance Method

# setReadHandler(\_:maxDatagrams:)

Set a read handler for datagrams.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func setReadHandler(
    _ handler: @escaping ([Data]?, (any Error)?) -> Void,
    maxDatagrams: Int
)
```

Deprecated

Use the nw_connection_receive(_:_:_:_:) function from the Network framework instead.

## Parameters 

`handler`  

A handler called when datagrams have been read, or when an error has occurred.

`maxDatagrams`  

The maximum number of datagrams to send to the handler.

## Discussion

Reads will be scheduled by the system, so this method only needs to be called once for a session.

## See Also

### Transferring data

func writeDatagram(Data, completionHandler: ((any Error)?) -> Void)

Write a single datagram.

Deprecated

func writeMultipleDatagrams([Data], completionHandler: ((any Error)?) -> Void)

Write multiple datagrams.

Deprecated

var maximumDatagramLength: Int

The maximum size of a datagram to be written currently.

Deprecated

