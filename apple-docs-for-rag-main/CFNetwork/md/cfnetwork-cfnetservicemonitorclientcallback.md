

- CFNetwork
-  CFNetServiceMonitorClientCallBack 

Type Alias

# CFNetServiceMonitorClientCallBack

Defines a pointer to the callback function that is to be called when a monitored record type changes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
typealias CFNetServiceMonitorClientCallBack = (CFNetServiceMonitor, CFNetService?, CFNetServiceMonitorType, CFData?, UnsafeMutablePointer?, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`theMonitor`  

CFNetServiceMonitor for which the callback is being called.

`theService`  

CFNetService for which the callback is being called.

`typeInfo`  

Type of record that changed. For possible values, see CFNetServiceMonitorType.

`rdata`  

Contents of the record that changed.

`error`  

Pointer to CFStreamError structure whose `error` field contains an error code if an error occurred.

`info`  

Arbitrary pointer to the user-defined data that was specified in the `info` field of the `CFNetServiceClientContext` structure when the monitor was created by CFNetServiceMonitorCreate(_:_:_:_:).

## Discussion

If you name your callback `MyNetServiceMonitorClientCallBack`, you would declare it like this:

### Discussion

The callback function will be called when the monitored record type changes or when the monitor is stopped by calling CFNetServiceMonitorStop(_:_:).

## See Also

### Data Types

typealias CFHostClientCallBack

Defines a pointer to the callback function that is called when an asynchronous resolution of a CFHost completes or an error occurs for an asynchronous CFHost resolution.

typealias CFNetServiceBrowserClientCallBack

Defines a pointer to the callback function for a CFNetServiceBrowser.

typealias CFNetServiceClientCallBack

Defines a pointer to the callback function for a CFNetService.

typealias CFNetDiagnosticStatus

A CFIndex type that is used to return status values from `CFNetDiagnostic` status and diagnostic functions. For a list of possible values, see CFNetDiagnosticStatusValues.

Deprecated

