

- Video Subscriber Account
- VSAccountMetadata
-  verificationData 

Instance Property

# verificationData

Data you use to verify that the response came from the account provider.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
var verificationData: Data? { get }
```

## Discussion

Use the data in this property to cryptographically verify that samlAttributeQueryResponse came from the account provider.

## See Also

### Getting App Authentication Info

var accountProviderResponse: VSAccountProviderResponse?

The response from the account provider.

var samlAttributeQueryResponse: String?

The SAML response from the account provider.

