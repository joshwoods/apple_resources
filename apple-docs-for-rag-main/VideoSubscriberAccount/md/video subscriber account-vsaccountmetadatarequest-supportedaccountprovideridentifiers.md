

- Video Subscriber Account
- VSAccountMetadataRequest
-  supportedAccountProviderIdentifiers 

Instance Property

# supportedAccountProviderIdentifiers

A list of identifiers for TV providers that your app supports.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
var supportedAccountProviderIdentifiers: [String] { get set }
```

## Discussion

Use this property to specify which TV providers receive the request. An empty list indicates that your app supports all TV providers in the region.

## See Also

### Requesting App-Level Authentication

var attributeNames: [String]

The SAML attributes that your app sends to the account provider.

var channelIdentifier: String?

The channel identifier for the request.

var supportedAuthenticationSchemes: [VSAccountProviderAuthenticationScheme]

A collection of authentication schemes your app supports for this request.

var verificationToken: String?

A token that your app sends to an account provider to identify itself.

