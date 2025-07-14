

- Network Extension
- NWUDPSession
-  maximumDatagramLength Deprecated

Instance Property

# maximumDatagramLength

The maximum size of a datagram to be written currently.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var maximumDatagramLength: Int { get }
```

Deprecated

Use the nw_connection_get_maximum_datagram_size(_:) function from the Network framework instead.

## Discussion

If a datagram is written with a longer length than `maximumDatagramLength`, the datagram may be fragmented or encounter an error. Note that this value is not guaranteed to be the maximum datagram length for end-to-end communication across the network. Use Key-Value Observing to watch this property.

## See Also

### Transferring data

func setReadHandler(([Data]?, (any Error)?) -> Void, maxDatagrams: Int)

Set a read handler for datagrams.

Deprecated

func writeDatagram(Data, completionHandler: ((any Error)?) -> Void)

Write a single datagram.

Deprecated

func writeMultipleDatagrams([Data], completionHandler: ((any Error)?) -> Void)

Write multiple datagrams.

Deprecated

