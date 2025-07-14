

- CFNetwork
-  CFNetServiceClientCallBack 

Type Alias

# CFNetServiceClientCallBack

Defines a pointer to the callback function for a CFNetService.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
typealias CFNetServiceClientCallBack = (CFNetService, UnsafeMutablePointer?, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`theService`  

CFNetService associated with this callback function.

`error`  

Pointer to a CFStreamError structure whose `error` field contain may contain an error code.

`info`  

User-defined context information. The value of `info` is the same as the value of the `info` field of the CFNetServiceClientContext structure that was provided when CFNetServiceSetClient(_:_:_:) was called for the CFNetService associated with this callback function.

## Discussion

If you name your callback `MyNetServiceClientCallBack`, you would declare it like this:

### Discussion

Your callback function will be called when there are results of resolving a CFNetService to report or when there are registration errors to report. In the case of resolution, if the service has more than one IP address, your callback will be called once for each address.

## See Also

### Data Types

typealias CFHostClientCallBack

Defines a pointer to the callback function that is called when an asynchronous resolution of a CFHost completes or an error occurs for an asynchronous CFHost resolution.

typealias CFNetServiceBrowserClientCallBack

Defines a pointer to the callback function for a CFNetServiceBrowser.

typealias CFNetServiceMonitorClientCallBack

Defines a pointer to the callback function that is to be called when a monitored record type changes.

typealias CFNetDiagnosticStatus

A CFIndex type that is used to return status values from `CFNetDiagnostic` status and diagnostic functions. For a list of possible values, see CFNetDiagnosticStatusValues.

Deprecated

