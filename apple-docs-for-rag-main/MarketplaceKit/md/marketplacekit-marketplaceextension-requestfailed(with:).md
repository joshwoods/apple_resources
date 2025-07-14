

- MarketplaceKit
- MarketplaceExtension
-  requestFailed(with:) 

Instance Method

# requestFailed(with:)

Handles when iOS receives an unexpected response from your web server.

iOS 17.4+iPadOS 17.4+

``` source
func requestFailed(with response: HTTPURLResponse) -> Bool
```

**Required**

## Parameters 

`response`  

An object that contains details of the response, such as the status code.

## Mentioned in 

Reauthenticating a person to manage apps

Installing apps from an alternative marketplace

## Discussion

iOS invokes your implementation of this callback when it receives anything but an OK status from your marketplace endpoints. Your implementation performs the necessary action according to the given status code. Your server might be down or it might return a code that indicates that the person needs to reauthenticate, if for example, their access token expires.

For more information, see Installing apps from an alternative marketplace.

