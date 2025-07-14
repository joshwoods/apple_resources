

- StoreKit Test
- SKAdTestPostback
-  postbackSequenceIndex 

Instance Property

# postbackSequenceIndex

The position of this postback among all postbacks for an ad impression.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+

``` source
var postbackSequenceIndex: Int { get }
```

## Discussion

For more information about receiving time-delayed postbacks for an ad impression, see Receiving postbacks in multiple conversion windows.

## See Also

### Getting general information

var version: SKAdTestPostbackVersion

The SKAdNetwork version that the postback uses.

var transactionIdentifier: String

A unique transaction identifier that the system generates.

var isRegistered: Bool

A Boolean value that indicates whether the postback is registered in the testing environment.

var isRedownload: Bool

A Boolean value that indicates whether the user redownloaded and reinstalled the app.

