

- StoreKit Test
- SKAdTestPostbackResponse
-  error 

Instance Property

# error

An error the test session reports if sending a test postbacks fails.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
var error: (any Error)? { get set }
```

## Discussion

If the test session encounters an error when attempting to send the test postback with flushPostbacks(responses:), this property contains an SKAdTestError error.

## See Also

### Getting Postback Responses

var didSucceed: Bool

A Boolean value that indicates whether the system successfully delivered the test postback.

var httpResponse: HTTPURLResponse?

The HTTP response from the server receiving the test postback.

