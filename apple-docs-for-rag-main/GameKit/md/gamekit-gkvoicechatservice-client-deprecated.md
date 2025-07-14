

- GameKit
- GKVoiceChatService
-  client Deprecated

Instance Property

# client

An object that the voice chat service uses to communicate with remote participants.

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
unowned(unsafe) var client: (any GKVoiceChatClient)! { get set }
```

Deprecated

No longer supported.

## Discussion

The client’s chief responsibility is to provide a network connection that the voice chat service can use to connect to another participant.

