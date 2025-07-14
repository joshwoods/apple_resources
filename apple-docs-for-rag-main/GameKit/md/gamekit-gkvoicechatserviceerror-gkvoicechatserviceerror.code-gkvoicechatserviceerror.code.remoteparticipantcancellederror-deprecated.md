

- GameKit
- GKVoiceChatServiceError
- GKVoiceChatServiceError.Code
-  GKVoiceChatServiceError.Code.remoteParticipantCancelledError Deprecated

Case

# GKVoiceChatServiceError.Code.remoteParticipantCancelledError

A remote participant attempted to start a voice chat, then canceled.

tvOS 9.0–18.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
case remoteParticipantCancelledError
```

Deprecated

No longer supported

## See Also

### Constants

case internalError

A serious error occurred inside the voice chat service.

Deprecated

case noRemotePacketsError

The voice chat service stopped receiving packets from the remote participant.

Deprecated

case unableToConnectError

The voice chat service was unable to establish a connection with another user.

Deprecated

case remoteParticipantHangupError

The remote participant in a voice chat stopped the chat.

Deprecated

case invalidCallIDError

The voice chat service didn’t recognize the call identifier.

Deprecated

case audioUnavailableError

The audio hardware is unavailable to the voice chat service.

Deprecated

case uninitializedClientError

The application did not set a client before calling voice chat service methods.

Deprecated

case clientMissingRequiredMethodsError

The voice chat service did not find an expected method defined by the client.

Deprecated

case remoteParticipantBusyError

The remote participant is already connected to a voice chat.

Deprecated

case remoteParticipantResponseInvalidError

Invalid data was received from a remote participant.

Deprecated

case remoteParticipantDeclinedInviteError

A remote participant declined an invitation.

Deprecated

case methodCurrentlyInvalidError

A method on the voice chat service was called when it was not allowed to be called (for example, attempting to connect when the voice chat service was already connected).

Deprecated

case networkConfigurationError

The voice chat service had problems accessing the network.

Deprecated

case unsupportedRemoteVersionError

The other participant is running a different version of the voice chat service.

Deprecated

case outOfMemoryError

The voice chat service was unable to allocate memory required to operate.

Deprecated

