

- CryptoTokenKit
- TKSmartCardUserInteraction
-  run(reply:) 

Instance Method

# run(reply:)

Runs the user interaction and asynchronously receives a reply.

iOSiPadOSMac Catalyst 13.1+macOS 10.11+tvOSvisionOSwatchOS

``` source
func run(reply: @escaping (Bool, (any Error)?) -> Void)
```

``` source
func run() async throws -> Bool
```

## Parameters 

`reply`  

success  
Whether the user interaction was successful.

error  
Contains information about the the error that occurred during the user interaction.

The `NSError` object is created in the TKErrorDomain domain with a code in the TKError.Code enumeration.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func run() async throws -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Starting and Stopping

func cancel() -> Bool

Attempts to cancel an interaction started by calling run(reply:). For certain interactions, cancellation may not be available.

