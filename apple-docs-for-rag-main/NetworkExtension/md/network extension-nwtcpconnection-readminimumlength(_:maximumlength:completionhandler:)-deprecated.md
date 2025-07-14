

- Network Extension
- NWTCPConnection
-  readMinimumLength(\_:maximumLength:completionHandler:) Deprecated

Instance Method

# readMinimumLength(\_:maximumLength:completionHandler:)

Read the requested range of bytes.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func readMinimumLength(
    _ minimum: Int,
    maximumLength maximum: Int,
    completionHandler completion: @escaping (Data?, (any Error)?) -> Void
)
```

Deprecated

Use the nw_connection_receive(_:_:_:_:) function from the Network framework instead.

## Parameters 

`minimum`  

The minimum number of bytes the caller wants to read.

`maximum`  

The maximum number of bytes the caller wants to read.

`completion`  

The completion handler to be invoked when data has been read or an error occurred.

## Discussion

The completion handler will be invoked when:

- The exact number of requested bytes have been read; `data` will be non-`nil`.

- Fewer than the requested number of bytes, or no bytes, have been read, and the connection’s read side has been closed. `data` might be `nil`, depending on whether there was any data to be read when the connection’s read side was closed.

- Some fatal error has occurred, returned in `error`, and `data` will be nil.

To know when to schedule a read again, check for the condition whether an error has occurred.

For better performance, the caller should pick the effective minimum and maximum lengths. For example, if the caller absolutely needs a specific number of bytes before it can make any progress, use that value as the minimum. The maximum bytes can be the upperbound that the caller wants to read. Typically, the minimum length can be the caller protocol fixed-size header and the maximum length can be the maximum size of the payload or the size of the current read buffer.

## See Also

### Transferring data

func readLength(Int, completionHandler: (Data?, (any Error)?) -> Void)

Read a certain number of bytes on a connection.

Deprecated

func write(Data, completionHandler: ((any Error)?) -> Void)

Write the data to the connection.

Deprecated

func writeClose()

Close the connection for writing.

Deprecated

