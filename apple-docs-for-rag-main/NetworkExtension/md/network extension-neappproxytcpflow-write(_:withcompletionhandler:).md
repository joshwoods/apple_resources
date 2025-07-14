

- Network Extension
- NEAppProxyTCPFlow
-  write(\_:withCompletionHandler:) 

Instance Method

# write(\_:withCompletionHandler:)

Write data to the flow.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func write(
    _ data: Data,
    withCompletionHandler completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func write(_ data: Data) async throws
```

## Parameters 

`data`  

An NSData object containing the data to write.

`completionHandler`  

A block that will be executed by the system on an internal system thread when the data is written into the receive buffer of the socket associated with the flow. The caller should use this callback as an indication that it is possible to write more data to the flow without using up excessive buffer memory. If an error occurs while writing the data then a non-nil NSError object is passed to the block. See `NEAppProxyFlowError` in NEAppProxyFlow for a list of possible errors.

## Mentioned in 

Handling Flow Copying

## See Also

### Handling flow data

func readData(completionHandler: (Data?, (any Error)?) -> Void)

Read data from the flow.

