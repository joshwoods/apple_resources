

- Video Subscriber Account
- VSAccountProviderResponse
-  body 

Instance Property

# body

The raw response from the provider.

iOS 10.2+iPadOS 10.2+macOStvOS 10.1+visionOS 1.0+

``` source
var body: String? { get }
```

## Discussion

This property is `nil` if the response contains security-sensitive information.

## See Also

### Getting Response Info

var authenticationScheme: VSAccountProviderAuthenticationScheme

The authentication scheme type of the response.

var status: String?

The status code for the response.

