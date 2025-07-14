

- Network Extension
- NWTCPConnection
-  writeClose() Deprecated

Instance Method

# writeClose()

Close the connection for writing.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func writeClose()
```

Deprecated

Use the nw_connection_send(_:_:_:_:_:) function from the Network framework instead.

## Discussion

Close this connection’s write side such that further write requests won’t succeed. Note that this has the effect of closing the read side of the peer connection. When the connection’s read side and write side are closed, the connection is considered disconnected and will transition to the appropriate state.

## See Also

### Transferring data

func readMinimumLength(Int, maximumLength: Int, completionHandler: (Data?, (any Error)?) -> Void)

Read the requested range of bytes.

Deprecated

func readLength(Int, completionHandler: (Data?, (any Error)?) -> Void)

Read a certain number of bytes on a connection.

Deprecated

func write(Data, completionHandler: ((any Error)?) -> Void)

Write the data to the connection.

Deprecated

