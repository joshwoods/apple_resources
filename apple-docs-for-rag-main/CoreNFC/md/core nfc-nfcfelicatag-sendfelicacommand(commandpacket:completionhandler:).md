

- Core NFC
- NFCFeliCaTag
-  sendFeliCaCommand(commandPacket:completionHandler:) 

Instance Method

# sendFeliCaCommand(commandPacket:completionHandler:)

Sends the FeliCa command packet data to the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func sendFeliCaCommand(
    commandPacket: Data,
    completionHandler: @escaping (Data, (any Error)?) -> Void
)
```

``` source
func sendFeliCaCommand(commandPacket: Data) async throws -> Data
```

**Required**

