

- GameKit
- GKError
- GKError.Code
-  GKError.Code.gameSessionRequestInvalid 

Case

# GKError.Code.gameSessionRequestInvalid

The properties of the game session request are impossible to fulfill.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
case gameSessionRequestInvalid
```

## Discussion

For example, the maximum number of requested players is greater than the maximum number of allowed players.

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

case invalidParameter

The system can’t complete the requested operation because one or more parameters are invalid.

case apiNotAvailable

The system can’t complete the requested operation because the API isn’t available.

case connectionTimeout

The system can’t complete the requested operation because the connection timed out.

case apiObsolete

The system can’t complete the requested operation because Apple deprecated the API.

