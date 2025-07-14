

- UIKit
- UIPasteConfiguration
-  init() 

Initializer

# init()

Initializes a new paste configuration.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init()
```

## Return Value

A paste configuration that has no acceptable uniform type identifiers (UTIs).

## Discussion

Use this initializer to create a paste configuration that has an empty acceptableTypeIdentifiers array. After you create the paste configuration, you can use its addAcceptableTypeIdentifiers(_:) method or addTypeIdentifiers(forAccepting:) method to add acceptable UTIs to the array.

## See Also

### Initializing a paste configuration

convenience init(acceptableTypeIdentifiers: [String])

Initializes a new paste configuration with a specified array of acceptable UTIs.

convenience init(forAccepting: any NSItemProviderReading.Type)

Initializes a new paste configuration with the UTIs declared as supported by a specified class.

convenience init&lt;T>(forAccepting: T.Type)

