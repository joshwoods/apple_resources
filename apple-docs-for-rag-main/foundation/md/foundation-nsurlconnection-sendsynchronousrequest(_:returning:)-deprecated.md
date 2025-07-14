

- Foundation
- NSURLConnection
-  sendSynchronousRequest(\_:returning:) Deprecated

Type Method

# sendSynchronousRequest(\_:returning:)

Performs a synchronous load of the specified URL request.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.3–10.11DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func sendSynchronousRequest(
    _ request: URLRequest,
    returning response: AutoreleasingUnsafeMutablePointer?
) throws -> Data
```

Deprecated

Use \[NSURLSession dataTaskWithRequest:completionHandler:\] (see NSURLSession.h

## Parameters 

`request`  

The URL request to load. The `request` object is deep-copied as part of the initialization process. Changes made to `request` after this method returns do not affect the request that is used for the loading process.

`response`  

Out parameter for the URL response returned by the server.

## Return Value

The downloaded data for the URL request. Returns `nil` if a connection could not be created or if the download fails.

## Discussion

A synchronous load is built on top of the asynchronous loading code made available by the class. The calling thread is blocked while the asynchronous loading system performs the URL load on a thread spawned specifically for this load request. No special threading or run loop configuration is necessary in the calling thread in order to perform a synchronous load.

Important

Because this call can potentially take several minutes to complete (particularly when using a cellular network in iOS), you should never call this function from the main thread of your application. Doing so may cause a `0x8badf00d` exception with the main thread at `mach_msg_trap`. The solution is to migrate to URL loading using URLSession.

If authentication is required in order to download the request, the required credentials must be specified as part of the URL. If authentication fails, or credentials are missing, the connection will attempt to continue without credentials.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

