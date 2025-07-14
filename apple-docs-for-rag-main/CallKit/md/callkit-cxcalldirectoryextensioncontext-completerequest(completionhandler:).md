

- CallKit
- CXCallDirectoryExtensionContext
-  completeRequest(completionHandler:) 

Instance Method

# completeRequest(completionHandler:)

Completes the request to the extension context.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+

``` source
func completeRequest(completionHandler completion: ((Bool) -> Void)? = nil)
```

``` source
func completeRequest() async -> Bool
```

## Parameters 

`completion`  

A block to be executed after the request to the extension context is completed.

expired  
Whether the receiver expired during the request.

If true, then any identification or blocking entries added by the extension context were not added to the extension.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func completeRequest() async -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Call this method on the instance of CXCallDirectoryExtensionContext passed as an argument to the block parameter of the CXCallDirectoryProvider instance method beginRequest(with:). This method should be called once at the end of the block.

## See Also

### Completing Requests

var isIncremental: Bool

A Boolean value that indicates whether the request provides data incrementally.

