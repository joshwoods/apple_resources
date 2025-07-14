

- UIKit
- UIPasteConfiguration
-  init(forAccepting:) 

Initializer

# init(forAccepting:)

iOS 11.0+iPadOS 11.0+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
convenience init(forAccepting _: T.Type) where T : _ObjectiveCBridgeable, T._ObjectiveCType : NSItemProviderReading
```

## See Also

### Initializing a paste configuration

init()

Initializes a new paste configuration.

convenience init(acceptableTypeIdentifiers: [String])

Initializes a new paste configuration with a specified array of acceptable UTIs.

convenience init(forAccepting: any NSItemProviderReading.Type)

Initializes a new paste configuration with the UTIs declared as supported by a specified class.

