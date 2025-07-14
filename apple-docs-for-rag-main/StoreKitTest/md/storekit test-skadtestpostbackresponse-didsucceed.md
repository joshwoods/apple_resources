

- StoreKit Test
- SKAdTestPostbackResponse
-  didSucceed 

Instance Property

# didSucceed

A Boolean value that indicates whether the system successfully delivered the test postback.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
var didSucceed: Bool { get set }
```

## Discussion

The value is `true` if the system successfully delivered the test postback and received an HTTP 200 response.

## See Also

### Getting Postback Responses

var httpResponse: HTTPURLResponse?

The HTTP response from the server receiving the test postback.

var error: (any Error)?

An error the test session reports if sending a test postbacks fails.

