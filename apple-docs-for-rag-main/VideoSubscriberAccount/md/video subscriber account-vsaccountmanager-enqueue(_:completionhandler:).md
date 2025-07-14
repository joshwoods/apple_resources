

- Video Subscriber Account
- VSAccountManager
-  enqueue(\_:completionHandler:) 

Instance Method

# enqueue(\_:completionHandler:)

Submits a request for subscriber account information.

iOS 10.0+iPadOS 10.0+tvOS 10.0+visionOS 1.0+

``` source
func enqueue(
    _ request: VSAccountMetadataRequest,
    completionHandler: @escaping (VSAccountMetadata?, (any Error)?) -> Void
) -> VSAccountManagerResult
```

## Parameters 

`request`  

A VSAccountMetadataRequest object that contains the information that your app requests.

`completionHandler`  

The closure that the account manager executes after the request completes. This closure has no return value and takes the following parameters:

metadata  
A VSAccountMetadata object that contains the requested information if the request was successful.

error  
An error object that contains information about a problem, or `nil` if the operation completed successfully.

## Return Value

Returns a VSAccountManagerResult object that your app can use with cancel() to cancel the request.

## See Also

### Enqueuing Requests

class VSAccountMetadataRequest

An object that specifies what subscriber account information your app retrieves.

class VSAccountMetadata

A collection of information for a subscriber’s account.

class VSAccountManagerResult

An object that represents a request made for subscriber account information.

class VSAccountProviderResponse

An object that contains the response from the account provider.

struct VSAccountProviderAuthenticationScheme

Authentication schemes for account provider requests and responses.

