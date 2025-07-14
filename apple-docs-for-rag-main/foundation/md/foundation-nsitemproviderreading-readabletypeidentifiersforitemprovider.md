

- Foundation
- NSItemProviderReading
-  readableTypeIdentifiersForItemProvider 

Type Property

# readableTypeIdentifiersForItemProvider

An array of UTI strings representing the data types supported by the class.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
static var readableTypeIdentifiersForItemProvider: [String] { get }
```

**Required**

## Discussion

Provide uniform type identifiers (UTIs) in order from highest fidelity to lowest. If your app employs a native data representation, place that first in the array.

