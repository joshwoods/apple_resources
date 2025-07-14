

- Core NFC
- CardSession
-  init() 

Initializer

# init()

Creates a contactless card session.

iOS 17.4+iPadOS 17.4+

``` source
init() async throws
```

## Discussion

Creating a card session depends on the following conditions:

- The device is eligible to use a card session.

- The person using the app has accepted the app’s request to use a card session.

Tip

Query the isSupported and isEligible properties before calling this initializer to avoid showing a system card session UI on ineligible devices.

This initializer throws an error of type CardSession.Error if it can’t create a card session. Possible error conditions are:

- CardSession.Error.accessNotAccepted

- CardSession.Error.systemEligibilityFailed

- CardSession.Error.radioDisabled

- CardSession.Error.systemNotAvailable

## See Also

### Creating a card session

enum Error

An error type that indicates problems with a card session.

