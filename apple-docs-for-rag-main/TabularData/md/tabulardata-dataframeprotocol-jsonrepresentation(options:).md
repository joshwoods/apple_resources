

- TabularData
- DataFrameProtocol
-  jsonRepresentation(options:) 

Instance Method

# jsonRepresentation(options:)

Generates a JSON data instance of the data frame.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func jsonRepresentation(options: JSONWritingOptions = .init()) throws -> Data
```

## Parameters 

`options`  

A JSONWritingOptions instance.

