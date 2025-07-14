

- StoreKit Test
- SKAdTestPostbackResponse
-  httpResponse 

Instance Property

# httpResponse

The HTTP response from the server receiving the test postback.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
var httpResponse: HTTPURLResponse? { get set }
```

## Discussion

This property contains your server’s full HTTP response.

## See Also

### Getting Postback Responses

var didSucceed: Bool

A Boolean value that indicates whether the system successfully delivered the test postback.

var error: (any Error)?

An error the test session reports if sending a test postbacks fails.

