

- StoreKit Test
-  SKAdTestPostbackResponse 

Class

# SKAdTestPostbackResponse

The status and error information for a postback that the system sends in the testing environment.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
class SKAdTestPostbackResponse
```

## Topics

### Getting Postback Responses

var didSucceed: Bool

A Boolean value that indicates whether the system successfully delivered the test postback.

var httpResponse: HTTPURLResponse?

The HTTP response from the server receiving the test postback.

var error: (any Error)?

An error the test session reports if sending a test postbacks fails.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Ad impression and postback testing

Testing and validating ad impression signatures and postbacks for SKAdNetwork

Validate your ad impressions and test your postbacks by creating unit tests using the StoreKit Test framework.

class SKAdTestSession

The class you use to test ad impressions and postbacks in Xcode.

class SKAdTestPostback

A test postback that contains ad conversion information in the testing environment.

struct SKAdTestPostbackVersion

A constant that indicates the postback version.

