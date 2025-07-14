

- GameKit
- GKError
- GKError.Code
-  GKError.Code.invalidParameter 

Case

# GKError.Code.invalidParameter

The system can’t complete the requested operation because one or more parameters are invalid.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
case invalidParameter
```

## Discussion

For example, this error code may be returned if your application attempts to post a score and provides a category string that does not match a category you configured for your leaderboards in App Store Connect.

## See Also

### Communication Errors

case unknown

The system can’t complete the requested operation due to an unknown error.

case cancelled

The system canceled the requested operation or the user disabled it.

case communicationsFailure

The system can’t complete the requested operation due to an error communicating with the server.

case invalidPlayer

The system can’t complete the requested operation because the player is invalid.

case gameSessionRequestInvalid

The properties of the game session request are impossible to fulfill.

case apiNotAvailable

The system can’t complete the requested operation because the API isn’t available.

case connectionTimeout

The system can’t complete the requested operation because the connection timed out.

case apiObsolete

The system can’t complete the requested operation because Apple deprecated the API.

