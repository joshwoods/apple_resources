

- PassKit (Apple Pay and Wallet)
- AsyncShareablePassConfiguration
-  AsyncShareablePassConfiguration.Result 

Enumeration

# AsyncShareablePassConfiguration.Result

PassKitSwiftUIiOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
enum Result
```

## Topics

### Enumeration Cases

case failure(any Error)

case loading

case success(PKAddShareablePassConfiguration)

## Relationships

### Conforms To

- Sendable

## See Also

### Creating the configuration

init(metadata: [PKShareablePassMetadata], action: PKAddShareablePassConfigurationPrimaryAction, content: (AsyncShareablePassConfiguration&lt;Content>.Result) -> Content)

