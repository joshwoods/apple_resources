

- StoreKit Test
- SKAdTestPostback
-  transactionIdentifier 

Instance Property

# transactionIdentifier

A unique transaction identifier that the system generates.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
var transactionIdentifier: String { get }
```

## Discussion

The system generates this value when you call setPostbacks(_:). This value is an empty string otherwise.

Use this value to match the test postback with the response you receive from flushPostbacks(responses:).

## See Also

### Getting general information

var version: SKAdTestPostbackVersion

The SKAdNetwork version that the postback uses.

var postbackSequenceIndex: Int

The position of this postback among all postbacks for an ad impression.

var isRegistered: Bool

A Boolean value that indicates whether the postback is registered in the testing environment.

var isRedownload: Bool

A Boolean value that indicates whether the user redownloaded and reinstalled the app.

