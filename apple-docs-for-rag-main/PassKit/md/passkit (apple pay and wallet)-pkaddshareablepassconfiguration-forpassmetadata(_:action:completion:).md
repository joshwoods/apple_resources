

- PassKit (Apple Pay and Wallet)
- PKAddShareablePassConfiguration
-  forPassMetadata(\_:action:completion:) 

Type Method

# forPassMetadata(\_:action:completion:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOSvisionOS 1.0+

``` source
class func forPassMetadata(
    _ passMetadata: [PKShareablePassMetadata],
    action: PKAddShareablePassConfigurationPrimaryAction,
    completion: @escaping (PKAddShareablePassConfiguration?, (any Error)?) -> Void
)
```

``` source
class func forPassMetadata(
    _ passMetadata: [PKShareablePassMetadata],
    action: PKAddShareablePassConfigurationPrimaryAction
) async throws -> PKAddShareablePassConfiguration
```

