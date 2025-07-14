

- MarketplaceKit
- MarketplaceExtension
-  additionalHeaders(for:account:) 

Instance Method

# additionalHeaders(for:account:)

Adds information to the request header for communications from the operating system to your marketplace endpoints.

iOS 17.4+iPadOS 17.4+

``` source
func additionalHeaders(
    for request: URLRequest,
    account: String
) -> [String : String]?
```

**Required**

## Parameters 

`request`  

A request that contains a header to which you add information.

`account`  

Authentication information about the signed-in person.

## Mentioned in 

Reauthenticating a person to manage apps

Installing apps from an alternative marketplace

## Discussion

The operating system invokes your implementation of this callback before sending a request to your marketplace endpoints. In this method, use addValue(_:forHTTPHeaderField:) to add to the header. The additions detail information that your marketplace server needs to authorize the request.

For more information, see Installing apps from an alternative marketplace.

