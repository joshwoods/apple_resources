

- CallKit
- CXProviderDelegate
-  provider(\_:execute:) 

Instance Method

# provider(\_:execute:)

Called when a transaction is executed by a call controller.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
optional func provider(
    _ provider: CXProvider,
    execute transaction: CXTransaction
) -> Bool
```

## Parameters 

`provider`  

The telephony provider.

`transaction`  

Contains the upcoming actions.

## Return Value

true if the `transaction` was handled; otherwise false.

## Discussion

Most delegates should not need to provide an implementation for this method. However, a delegate can implement this method to customize how transactions are handled. This method returns true to indicate that the custom implementation handled the transaction and returns false to have the provider execute the transaction normally—as if the delegate did not implement this method. For example, given a transaction consisting of a CXSetHeldCallAction object and a CXSetGroupCallAction object, the delegate may override this method to inject a 30 second wait and play hold music to the caller.

