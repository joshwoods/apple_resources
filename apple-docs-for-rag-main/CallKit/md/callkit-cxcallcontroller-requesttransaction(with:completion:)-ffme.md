

- CallKit
- CXCallController
-  requestTransaction(with:completion:) 

Instance Method

# requestTransaction(with:completion:)

Requests that the transaction that contains the specified action be asynchronously performed by the telephony provider.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+visionOS 1.0+watchOS 9.0+

``` source
func requestTransaction(
    with action: CXAction,
    completion: @escaping ((any Error)?) -> Void
)
```

``` source
func requestTransaction(with action: CXAction) async throws
```

## Parameters 

`action`  

The telephony action associated with a call object.

`completion`  

Code to be executed after the transaction is completed. The callback is executed on the queue specified when the call controller was initialized.

transaction  
The requested transaction.

error  
If an error occurred, an error object indicating how the transaction failed, otherwise `nil`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func requestTransaction(with action: CXAction) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Requesting Transactions

func request(CXTransaction, completion: ((any Error)?) -> Void)

Requests that the actions in the specified transaction be asynchronously performed by the telephony provider.

func requestTransaction(with: [CXAction], completion: ((any Error)?) -> Void)

Requests that the transaction that contains the specified actions be asynchronously performed by the telephony provider.

