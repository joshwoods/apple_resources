

- TabularData
- DataFrameProtocol
-  writeJSON(to:options:) 

Instance Method

# writeJSON(to:options:)

Creates a JSON file with the contents of the data frame.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func writeJSON(
    to url: URL,
    options: JSONWritingOptions = .init()
) throws
```

## Parameters 

`url`  

A location URL in the file system where the method saves the JSON file.

`options`  

A JSONWritingOptions instance.

