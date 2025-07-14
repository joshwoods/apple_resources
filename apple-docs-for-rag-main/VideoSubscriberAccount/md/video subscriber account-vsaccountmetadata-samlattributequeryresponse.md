

- Video Subscriber Account
- VSAccountMetadata
-  samlAttributeQueryResponse 

Instance Property

# samlAttributeQueryResponse

The SAML response from the account provider.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
var samlAttributeQueryResponse: String? { get }
```

## Discussion

This property is `nil` if you didn’t specify any SAML attributes in your VSAccountMetadataRequest object or if the user doesn’t have a valid authentication session with the account provider.

## See Also

### Getting App Authentication Info

var accountProviderResponse: VSAccountProviderResponse?

The response from the account provider.

var verificationData: Data?

Data you use to verify that the response came from the account provider.

