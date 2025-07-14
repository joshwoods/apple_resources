

- Network Extension
- NEAppProxyTCPFlow
-  readData(completionHandler:) 

Instance Method

# readData(completionHandler:)

Read data from the flow.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func readData(completionHandler: @escaping (Data?, (any Error)?) -> Void)
```

## Parameters 

`completionHandler`  

A block that will be executed by the system on an internal system thread when some data is read from the flow. The block is passed either the data that was read or a non-nil error if an error occurred. See `NEAppProxyFlowError` in NEAppProxyFlow for a list of possible errors. If the data parameter has a length of 0 then no data can be subsequently read from the flow.

Note

The completion handler is only called for the single read operation that was initiated by calling this method. If the caller wants to read more data then it should call this method again to schedule another read operation and another execution of the completion handler block.

## Mentioned in 

Handling Flow Copying

## See Also

### Handling flow data

func write(Data, withCompletionHandler: ((any Error)?) -> Void)

Write data to the flow.

