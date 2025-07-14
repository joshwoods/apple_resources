

- StoreKit Test
- SKAdTestPostback
-  version 

Instance Property

# version

The SKAdNetwork version that the postback uses.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
var version: SKAdTestPostbackVersion { get }
```

## Discussion

For information about the SKAdNetwork versions, See SKAdNetwork release notes.

## See Also

### Getting general information

var transactionIdentifier: String

A unique transaction identifier that the system generates.

var postbackSequenceIndex: Int

The position of this postback among all postbacks for an ad impression.

var isRegistered: Bool

A Boolean value that indicates whether the postback is registered in the testing environment.

var isRedownload: Bool

A Boolean value that indicates whether the user redownloaded and reinstalled the app.

