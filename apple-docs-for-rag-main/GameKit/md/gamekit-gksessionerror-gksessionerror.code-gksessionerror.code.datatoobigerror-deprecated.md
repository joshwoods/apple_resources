

- GameKit
- GKSessionError
- GKSessionError.Code
-  GKSessionError.Code.dataTooBigError Deprecated

Case

# GKSessionError.Code.dataTooBigError

The data your application attempted to send was too large for the session to transmit in a single call.

tvOS 9.0–18.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
case dataTooBigError
```

Deprecated

No longer supported

## See Also

### Constants

case invalidParameterError

A parameter had an unexpected value.

Deprecated

case peerNotFoundError

A peer with the specified `peerID` string could not be found.

Deprecated

case declinedError

The peer your application tried to connect to refused the connection.

Deprecated

case timedOutError

The operation could not be completed in the specified timeout period.

Deprecated

case cancelledError

A peer that invited the session to connect to them canceled the connection request.

Deprecated

case connectionFailedError

The attempt to establish a connection with another peer failed.

Deprecated

case connectionClosedError

The connection to another peer closed unexpectedly.

Deprecated

case notConnectedError

Reserved for future use.

Deprecated

case cannotEnableError

Bluetooth is not currently available.

Deprecated

case inProgressError

The peer your application attempted to connect to has already requested a connection to your session.

Deprecated

case connectivityError

An error occurred in the GKSession object’s connection code.

Deprecated

case transportError

An error occurred in the GKSession object’s transport code.

Deprecated

case internalError

A serious error occurred inside GKSession.

Deprecated

case unknownError

Reserved for when the error does not fit in another category above.

Deprecated

case systemError

An error occurred outside of the GKSession object’s control, such as memory allocation.

Deprecated

