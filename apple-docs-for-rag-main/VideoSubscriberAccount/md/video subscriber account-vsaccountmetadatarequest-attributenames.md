

- Video Subscriber Account
- VSAccountMetadataRequest
-  attributeNames 

Instance Property

# attributeNames

The SAML attributes that your app sends to the account provider.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
var attributeNames: [String] { get set }
```

## Discussion

Use this property to add an array of SAML attribute names to a SAML attribute query request.

## See Also

### Requesting App-Level Authentication

var channelIdentifier: String?

The channel identifier for the request.

var supportedAccountProviderIdentifiers: [String]

A list of identifiers for TV providers that your app supports.

var supportedAuthenticationSchemes: [VSAccountProviderAuthenticationScheme]

A collection of authentication schemes your app supports for this request.

var verificationToken: String?

A token that your app sends to an account provider to identify itself.

