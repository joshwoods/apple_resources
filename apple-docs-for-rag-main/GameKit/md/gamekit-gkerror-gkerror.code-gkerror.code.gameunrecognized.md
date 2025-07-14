

- GameKit
- GKError
- GKError.Code
-  GKError.Code.gameUnrecognized 

Case

# GKError.Code.gameUnrecognized

The system can’t complete the requested operation because Game Center doesn’t recognize the app.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
case gameUnrecognized
```

## Discussion

Ensure the app’s `bundleID` is correct.

## See Also

### Configuration Errors

case notSupported

The app doesn’t have Game Center enabled.

case appUnlisted

The system can’t complete the requested operation because the game isn’t available on the App Store.

