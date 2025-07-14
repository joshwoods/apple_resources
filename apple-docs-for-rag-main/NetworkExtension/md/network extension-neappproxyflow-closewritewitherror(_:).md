

- Network Extension
- NEAppProxyFlow
-  closeWriteWithError(\_:) 

Instance Method

# closeWriteWithError(\_:)

Close the flow for further write operations.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func closeWriteWithError(_ error: (any Error)?)
```

## Parameters 

`error`  

An NSError object indicating to the system the error that led to the closure. If the flow is not being closed due to an error, this parameter should be set to nil. See `NEAppProxyFlowError` below for a list of acceptable error codes.

## Mentioned in 

Handling Flow Copying

## See Also

### Managing the flow life cycle

func open(withLocalEndpoint: NWHostEndpoint?, completionHandler: ((any Error)?) -> Void)

Opens the flow, indicating to the system that the caller is ready to start receiving and sending data.

Deprecated

func closeReadWithError((any Error)?)

Close the flow for further read operations.

