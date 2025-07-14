

- UIKit
- UIPasteConfiguration
-  addTypeIdentifiers(forAccepting:) 

Instance Method

# addTypeIdentifiers(forAccepting:)

iOS 11.0+iPadOS 11.0+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
func addTypeIdentifiers(forAccepting aClass: T.Type) where T : _ObjectiveCBridgeable, T._ObjectiveCType : NSItemProviderReading
```

## See Also

### Adding acceptable type identifiers

func addAcceptableTypeIdentifiers([String])

Adds an array of UTI strings to a paste configuration, increasing the variety of types the paste configuration accepts.

func addTypeIdentifiers(forAccepting: any NSItemProviderReading.Type)

Expands the array of accepted UTIs for a paste configuration, based on those declared as supported by a specified class.

