

- Video Subscriber Account
- VSAccountMetadataRequest
-  forceAuthentication 

Instance Property

# forceAuthentication

A Boolean value that indicates whether the app ignores cached credentials.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
var forceAuthentication: Bool { get set }
```

## Discussion

If true, your app cannot use cached credentials; if false, your app attempts to use any available cached credentials.

## See Also

### Specifying Additional Options

var isInterruptionAllowed: Bool

A Boolean value that indicates whether your app can prompt the user to authenticate to complete the request.

var featuredAccountProviderIdentifiers: [String]

The providers your app lists prominently during authentication.

var localizedVideoTitle: String?

A short, user-presentable name for the video that the user wants to play.

var applicationAccountProviders: [VSAccountApplicationProvider]?

An array of application-specific providers to add to the list of account providers.

