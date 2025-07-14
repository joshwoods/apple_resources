

- StoreKit Test
- SKAdTestSession
-  setPostbacks(\_:) 

Instance Method

# setPostbacks(\_:)

Add test postbacks to the test session.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
func setPostbacks(_ postbacks: [SKAdTestPostback]) throws
```

## Parameters 

`postbacks`  

An array of one to six test postbacks you add to a test session. The first postback must always be the winning postback with a `didWin` value of `true`. There must be only one winning postback.

## Discussion

An error occurs if any of the test postbacks are invalid or if there’s an issue with the set of test postbacks. Otherwise, the test passes.

Create postbacks using the initializer for SKAdTestPostback, init(version:adNetworkIdentifier:adCampaignIdentifier:appStoreItemIdentifier:sourceAppStoreItemIdentifier:conversionValue:fidelityType:isRedownload:didWin:postbackURL:). Add the postbacks to the test session by calling setPostbacks(_:).

Calling setPostbacks(_:) overwrites previous postbacks in the test session, if any exist.

Include up to six test postbacks in your test session if you want to mimic the behavior of postbacks when users experience multiple ad impressions for the same app. For more information about attributions when there are multiple ad impressions, see Receiving ad attributions and postbacks.

The array of test postbacks in the test session need to follow the same rules that SKAdNetwork uses for postbacks, including:

- The `postbacks` array can only contain up to six postbacks.

- The first postback in the array must be the only winning postback in the array, with a `didWin` value of `true`.

- All postbacks, except the first postback in the array, have a `didWin` value of `false`.

## See Also

### Adding and sending postbacks

var postbacks: [SKAdTestPostback]

An array of test postbacks you set in the testing environment.

func flushPostbacks(responses: SKANTestPostbackResponseHandler)

Sends the test postbacks and handles the responses.

typealias SKANTestPostbackResponseHandler

A type that represents the test postback response handler.

