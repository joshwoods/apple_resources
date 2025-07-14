

- Core NFC
- NFCISO15693Tag
-  stayQuiet(completionHandler:) 

Instance Method

# stayQuiet(completionHandler:)

Sends a Stay Quiet command (0x02 command code), as defined in the ISO 15693-3 specification, to the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func stayQuiet(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
func stayQuiet() async throws
```

**Required**

