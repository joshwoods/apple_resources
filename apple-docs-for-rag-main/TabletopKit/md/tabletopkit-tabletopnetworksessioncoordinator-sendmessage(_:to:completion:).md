

- TabletopKit
- TabletopNetworkSessionCoordinator
-  sendMessage(\_:to:completion:) 

Instance Method

# sendMessage(\_:to:completion:)

visionOS 2.0+

``` source
func sendMessage(
    _ message: Data,
    to: Set,
    completion: @escaping (TabletopSendMessageResult) -> Void
)
```

**Required**

## See Also

### Sending messages between peers

func sendMessageUnreliably(Data, to: Set&lt;Self.Peer>, completion: (TabletopSendMessageResult) -> Void)

**Required**

