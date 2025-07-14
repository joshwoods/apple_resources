

- Video Subscriber Account
- VSAccountMetadataRequest
-  verificationToken 

Instance Property

# verificationToken

A token that your app sends to an account provider to identify itself.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
var verificationToken: String? { get set }
```

## Discussion

Account providers use this token to verify the identity of the requesting app.

## See Also

### Requesting App-Level Authentication

var attributeNames: [String]

The SAML attributes that your app sends to the account provider.

var channelIdentifier: String?

The channel identifier for the request.

var supportedAccountProviderIdentifiers: [String]

A list of identifiers for TV providers that your app supports.

var supportedAuthenticationSchemes: [VSAccountProviderAuthenticationScheme]

A collection of authentication schemes your app supports for this request.

