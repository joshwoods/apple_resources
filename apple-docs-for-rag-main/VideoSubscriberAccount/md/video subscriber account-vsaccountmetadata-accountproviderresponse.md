

- Video Subscriber Account
- VSAccountMetadata
-  accountProviderResponse 

Instance Property

# accountProviderResponse

The response from the account provider.

iOS 10.2+iPadOS 10.2+macOStvOS 10.1+visionOS 1.0+

``` source
var accountProviderResponse: VSAccountProviderResponse? { get }
```

## Discussion

This property is `nil` if you didn’t specify any attributes in your VSAccountMetadataRequest object or if the user doesn’t have a valid authentication session with the account provider.

## See Also

### Getting App Authentication Info

var samlAttributeQueryResponse: String?

The SAML response from the account provider.

var verificationData: Data?

Data you use to verify that the response came from the account provider.

