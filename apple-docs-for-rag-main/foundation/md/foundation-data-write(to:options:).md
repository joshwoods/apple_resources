

- Foundation
- Data
-  write(to:options:) 

Instance Method

# write(to:options:)

Writes the contents of the data buffer to a location.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func write(
    to url: URL,
    options: Data.WritingOptions = []
) throws
```

## Parameters 

`url`  

The location to write the data into.

`options`  

Options for writing the data. Default value is `[]`.

## See Also

### Reading and Writing Data

typealias ReadingOptions

Options to control the reading of data from a URL.

typealias WritingOptions

Options to control the writing of data to a URL.

