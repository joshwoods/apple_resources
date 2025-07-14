

- Video Subscriber Account
- VSAccountProviderResponse
-  authenticationScheme 

Instance Property

# authenticationScheme

The authentication scheme type of the response.

iOS 10.2+iPadOS 10.2+macOStvOS 10.1+visionOS 1.0+

``` source
var authenticationScheme: VSAccountProviderAuthenticationScheme { get }
```

## Discussion

This property identifies the authentication scheme the account provider used to construct the response. See VSAccountProviderAuthenticationScheme for a list of types.

## See Also

### Getting Response Info

var body: String?

The raw response from the provider.

var status: String?

The status code for the response.

