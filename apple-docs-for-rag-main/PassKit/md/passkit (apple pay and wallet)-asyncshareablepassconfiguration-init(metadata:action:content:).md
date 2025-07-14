

- PassKit (Apple Pay and Wallet)
- AsyncShareablePassConfiguration
-  init(metadata:action:content:) 

Initializer

# init(metadata:action:content:)

PassKitSwiftUIiOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
nonisolated
init(
    metadata: [PKShareablePassMetadata],
    action: PKAddShareablePassConfigurationPrimaryAction,
    @ViewBuilder content: @escaping (AsyncShareablePassConfiguration.Result) -> Content
)
```

## See Also

### Creating the configuration

enum Result

