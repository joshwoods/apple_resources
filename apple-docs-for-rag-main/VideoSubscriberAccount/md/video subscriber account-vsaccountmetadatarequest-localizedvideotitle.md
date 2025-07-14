

- Video Subscriber Account
- VSAccountMetadataRequest
-  localizedVideoTitle 

Instance Property

# localizedVideoTitle

A short, user-presentable name for the video that the user wants to play.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
var localizedVideoTitle: String? { get set }
```

## Discussion

Use this property to display a short localized name for the video your app will play if the request is successful. For example, `My Cool Movie` or `My Favorite Show S2 E5`.

A value is not required if your app isn’t sending the request to play a specific video.

## See Also

### Specifying Additional Options

var isInterruptionAllowed: Bool

A Boolean value that indicates whether your app can prompt the user to authenticate to complete the request.

var featuredAccountProviderIdentifiers: [String]

The providers your app lists prominently during authentication.

var forceAuthentication: Bool

A Boolean value that indicates whether the app ignores cached credentials.

var applicationAccountProviders: [VSAccountApplicationProvider]?

An array of application-specific providers to add to the list of account providers.

