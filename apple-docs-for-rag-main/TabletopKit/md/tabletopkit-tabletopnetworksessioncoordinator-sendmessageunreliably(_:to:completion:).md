

- TabletopKit
- TabletopNetworkSessionCoordinator
-  sendMessageUnreliably(\_:to:completion:) 

Instance Method

# sendMessageUnreliably(\_:to:completion:)

visionOS 2.0+

``` source
func sendMessageUnreliably(
    _ message: Data,
    to: Set,
    completion: @escaping (TabletopSendMessageResult) -> Void
)
```

**Required**

## See Also

### Sending messages between peers

func sendMessage(Data, to: Set&lt;Self.Peer>, completion: (TabletopSendMessageResult) -> Void)

**Required**

