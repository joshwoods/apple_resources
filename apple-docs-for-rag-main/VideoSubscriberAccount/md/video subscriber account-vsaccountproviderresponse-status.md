

- Video Subscriber Account
- VSAccountProviderResponse
-  status 

Instance Property

# status

The status code for the response.

iOS 10.2+iPadOS 10.2+macOStvOS 10.1+visionOS 1.0+

``` source
var status: String? { get }
```

## Discussion

This property is `nil` if the response doesn’t match an existing status type.

## See Also

### Getting Response Info

var authenticationScheme: VSAccountProviderAuthenticationScheme

The authentication scheme type of the response.

var body: String?

The raw response from the provider.

