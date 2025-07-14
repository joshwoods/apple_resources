

- Core Media I/O
- CMIOExtensionStreamSource
-  authorizedToStartStream(for:) 

Instance Method

# authorizedToStartStream(for:)

Determines whether to authorize an app to use this stream.

Mac Catalyst 15.4+macOS 12.3+

``` source
func authorizedToStartStream(for client: CMIOExtensionClient) -> Bool
```

**Required**

## Parameters 

`client`  

The client with authorization to check.

## Return Value

true if you authorize the app; otherwise, false.

## See Also

### Managing a Stream

func startStream() throws

Starts the stream of media data.

**Required**

func stopStream() throws

Stops the stream of media data.

**Required**

