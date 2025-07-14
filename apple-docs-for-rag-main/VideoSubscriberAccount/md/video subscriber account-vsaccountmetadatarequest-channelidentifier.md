

- Video Subscriber Account
- VSAccountMetadataRequest
-  channelIdentifier 

Instance Property

# channelIdentifier

The channel identifier for the request.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
var channelIdentifier: String? { get set }
```

## Discussion

This property identifies the app that is making the request. If you distribute multiple apps, use this identifier to communicate which app sent the request.

Note

This property is only for applications that use the SAML authentication scheme.

## See Also

### Requesting App-Level Authentication

var attributeNames: [String]

The SAML attributes that your app sends to the account provider.

var supportedAccountProviderIdentifiers: [String]

A list of identifiers for TV providers that your app supports.

var supportedAuthenticationSchemes: [VSAccountProviderAuthenticationScheme]

A collection of authentication schemes your app supports for this request.

var verificationToken: String?

A token that your app sends to an account provider to identify itself.

