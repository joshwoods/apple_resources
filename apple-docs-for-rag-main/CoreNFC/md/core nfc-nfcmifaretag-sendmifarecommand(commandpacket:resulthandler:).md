

- Core NFC
- NFCMiFareTag
-  sendMiFareCommand(commandPacket:resultHandler:) 

Instance Method

# sendMiFareCommand(commandPacket:resultHandler:)

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
func sendMiFareCommand(
    commandPacket command: Data,
    resultHandler: @escaping (Result) -> Void
)
```

