

- GameKit
- GKVoiceChatClient
-  participantID() Deprecated

Instance Method

# participantID()

Returns a string that uniquely identifies the local user.

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
func participantID() -> String
```

**Required**

## Return Value

A string that can be used by other participants to connect to the local user.

## Discussion

The client decides the format and meaning of the participant identifier.

