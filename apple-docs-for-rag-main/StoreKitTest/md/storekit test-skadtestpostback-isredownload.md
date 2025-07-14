

- StoreKit Test
- SKAdTestPostback
-  isRedownload 

Instance Property

# isRedownload

A Boolean value that indicates whether the user redownloaded and reinstalled the app.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
var isRedownload: Bool { get }
```

## Discussion

In the production environment, this value is `true` when the user redownloaded and reinstalled the app. In the testing environment, you set the value of this property when you create the test postback.

## See Also

### Getting general information

var version: SKAdTestPostbackVersion

The SKAdNetwork version that the postback uses.

var transactionIdentifier: String

A unique transaction identifier that the system generates.

var postbackSequenceIndex: Int

The position of this postback among all postbacks for an ad impression.

var isRegistered: Bool

A Boolean value that indicates whether the postback is registered in the testing environment.

