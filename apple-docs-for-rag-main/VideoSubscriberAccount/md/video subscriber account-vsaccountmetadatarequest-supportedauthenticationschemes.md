

- Video Subscriber Account
- VSAccountMetadataRequest
-  supportedAuthenticationSchemes 

Instance Property

# supportedAuthenticationSchemes

A collection of authentication schemes your app supports for this request.

iOS 10.2+iPadOS 10.2+macOStvOS 10.1+visionOS 1.0+

``` source
var supportedAuthenticationSchemes: [VSAccountProviderAuthenticationScheme] { get set }
```

## Discussion

Use this property to check if the authentication schemes your app supports are compatible with account providers. The default is `VSAccountProviderAuthenticationSchemeSAML`.

## See Also

### Requesting App-Level Authentication

var attributeNames: [String]

The SAML attributes that your app sends to the account provider.

var channelIdentifier: String?

The channel identifier for the request.

var supportedAccountProviderIdentifiers: [String]

A list of identifiers for TV providers that your app supports.

var verificationToken: String?

A token that your app sends to an account provider to identify itself.

