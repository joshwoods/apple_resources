

- UIKit
- UIPasteConfiguration
-  init(forAccepting:) 

Initializer

# init(forAccepting:)

Initializes a new paste configuration with the UTIs declared as supported by a specified class.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
convenience init(forAccepting aClass: any NSItemProviderReading.Type)
```

## Parameters 

`aClass`  

A class conforming to the NSItemProviderReading protocol.

## Return Value

A paste configuration initialized with acceptable uniform type identifiers (UTIs) supported by the specified class.

## Discussion

When you use this initializer, the property readableTypeIdentifiersForItemProvider, implemented on `aClass`, is used to determine the acceptable UTIs.

## See Also

### Initializing a paste configuration

init()

Initializes a new paste configuration.

convenience init(acceptableTypeIdentifiers: [String])

Initializes a new paste configuration with a specified array of acceptable UTIs.

convenience init&lt;T>(forAccepting: T.Type)

