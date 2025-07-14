

- StoreKit Test
- SKAdTestPostback
-  isRegistered 

Instance Property

# isRegistered

A Boolean value that indicates whether the postback is registered in the testing environment.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
var isRegistered: Bool { get }
```

## Discussion

To register a postback, call updatePostbackConversionValue(_:completionHandler:), or registerAppForAdNetworkAttribution().

## See Also

### Getting general information

var version: SKAdTestPostbackVersion

The SKAdNetwork version that the postback uses.

var transactionIdentifier: String

A unique transaction identifier that the system generates.

var postbackSequenceIndex: Int

The position of this postback among all postbacks for an ad impression.

var isRedownload: Bool

A Boolean value that indicates whether the user redownloaded and reinstalled the app.

