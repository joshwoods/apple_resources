

- Network Extension
- NWTCPConnection
-  readLength(\_:completionHandler:) Deprecated

Instance Method

# readLength(\_:completionHandler:)

Read a certain number of bytes on a connection.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func readLength(
    _ length: Int,
    completionHandler completion: @escaping (Data?, (any Error)?) -> Void
)
```

Deprecated

Use the nw_connection_receive(_:_:_:_:) function from the Network framework instead.

## Parameters 

`length`  

The exact number of bytes the caller wants to read.

`completion`  

The completion handler to be invoked when data has been read or an error occurred.

## Discussion

Read `length` number of bytes. See `readMinimumLength:maximumLength:completionHandler:` for a complete discussion of the callback behavior.

## See Also

### Transferring data

func readMinimumLength(Int, maximumLength: Int, completionHandler: (Data?, (any Error)?) -> Void)

Read the requested range of bytes.

Deprecated

func write(Data, completionHandler: ((any Error)?) -> Void)

Write the data to the connection.

Deprecated

func writeClose()

Close the connection for writing.

Deprecated

