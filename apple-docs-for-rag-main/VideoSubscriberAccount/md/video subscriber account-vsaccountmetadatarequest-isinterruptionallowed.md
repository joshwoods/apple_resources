

- Video Subscriber Account
- VSAccountMetadataRequest
-  isInterruptionAllowed 

Instance Property

# isInterruptionAllowed

A Boolean value that indicates whether your app can prompt the user to authenticate to complete the request.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
var isInterruptionAllowed: Bool { get set }
```

## See Also

### Specifying Additional Options

var featuredAccountProviderIdentifiers: [String]

The providers your app lists prominently during authentication.

var forceAuthentication: Bool

A Boolean value that indicates whether the app ignores cached credentials.

var localizedVideoTitle: String?

A short, user-presentable name for the video that the user wants to play.

var applicationAccountProviders: [VSAccountApplicationProvider]?

An array of application-specific providers to add to the list of account providers.

