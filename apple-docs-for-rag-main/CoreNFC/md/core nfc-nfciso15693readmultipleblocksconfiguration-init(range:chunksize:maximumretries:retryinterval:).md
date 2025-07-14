

- Core NFC
- NFCISO15693ReadMultipleBlocksConfiguration
-  init(range:chunkSize:maximumRetries:retryInterval:) 

Initializer

# init(range:chunkSize:maximumRetries:retryInterval:)

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
init(
    range: NSRange,
    chunkSize: Int,
    maximumRetries: Int,
    retryInterval: TimeInterval
)
```

## Parameters 

`range`  

Read range specify by the starting block index and the total number of blocks.

`chunkSize`  

Specify number of blocks parameter for the Read multiple blocks command.

`maximumRetries`  

Maximum number of retry attempt when tag response is not received.

`retryInterval`  

Time interval wait between each retry attempt.

