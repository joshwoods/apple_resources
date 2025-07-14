

- CFNetwork
-  CFNetServiceBrowserClientCallBack 

Type Alias

# CFNetServiceBrowserClientCallBack

Defines a pointer to the callback function for a CFNetServiceBrowser.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
typealias CFNetServiceBrowserClientCallBack = (CFNetServiceBrowser, CFOptionFlags, CFTypeRef?, UnsafeMutablePointer?, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`browser`  

The CFNetServiceBrowser associated with this callback function.

`flags`  

Flags conveying additional information. The `kCFNetServiceFlagIsDomain` bit is set if `domainOrService` contains a domain; if this bit is not set, `domainOrService` contains a CFNetService instance. For additional bit values, see `CFNetServiceBrowserClientCallBack Bit Flags`.

`domainOrService`  

A string containing a domain name if this callback function is being called as a result of calling CFNetServiceBrowserSearchForDomains(_:_:_:), or a CFNetService instance if this callback function is being called as a result calling CFNetServiceBrowserSearchForServices(_:_:_:_:).

`error`  

A pointer to a CFStreamError structure whose `error` field may contain an error code.

`info`  

User-defined context information. The value of `info` is the same as the value of the `info` field of the CFNetServiceClientContext structure that was provided when CFNetServiceBrowserCreate(_:_:_:) was called to create the CFNetServiceBrowser associated with this callback function.

## Discussion

If you name your callback `MyNetServiceBrowserClientCallBack`, you would declare it like this:

### Discussion

The callback function for a CFNetServiceBrowser is called one or more times when domains or services are found as the result of calling CFNetServiceBrowserSearchForDomains(_:_:_:) and CFNetServiceBrowserSearchForServices(_:_:_:_:).

## See Also

### Data Types

typealias CFHostClientCallBack

Defines a pointer to the callback function that is called when an asynchronous resolution of a CFHost completes or an error occurs for an asynchronous CFHost resolution.

typealias CFNetServiceClientCallBack

Defines a pointer to the callback function for a CFNetService.

typealias CFNetServiceMonitorClientCallBack

Defines a pointer to the callback function that is to be called when a monitored record type changes.

typealias CFNetDiagnosticStatus

A CFIndex type that is used to return status values from `CFNetDiagnostic` status and diagnostic functions. For a list of possible values, see CFNetDiagnosticStatusValues.

Deprecated

