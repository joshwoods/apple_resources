

- Network Extension
- NWTCPConnection
-  write(\_:completionHandler:) Deprecated

Instance Method

# write(\_:completionHandler:)

Write the data to the connection.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func write(
    _ data: Data,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

Deprecated

Use the nw_connection_send(_:_:_:_:_:) function from the Network framework instead.

## Parameters 

`data`  

The data object whose content will be written.

`completion`  

The completion handler to be invoked when the data content has been written or an error has occurred. If `error` is `nil`, the write succeeded and the caller can write more data.

## Discussion

Callers should wait until the `completionHandler` is executed before issuing another write.

## See Also

### Transferring data

func readMinimumLength(Int, maximumLength: Int, completionHandler: (Data?, (any Error)?) -> Void)

Read the requested range of bytes.

Deprecated

func readLength(Int, completionHandler: (Data?, (any Error)?) -> Void)

Read a certain number of bytes on a connection.

Deprecated

func writeClose()

Close the connection for writing.

Deprecated

