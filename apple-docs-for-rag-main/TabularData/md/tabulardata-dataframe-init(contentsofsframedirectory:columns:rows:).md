

- TabularData
- DataFrame
-  init(contentsOfSFrameDirectory:columns:rows:) 

Initializer

# init(contentsOfSFrameDirectory:columns:rows:)

Creates a data frame from a Turi Create scalable data frame.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    contentsOfSFrameDirectory url: URL,
    columns: [String]? = nil,
    rows: Range? = nil
) throws
```

## Parameters 

`url`  

A URL to an `SFrame` directory.

`columns`  

An array of column names; Set to `nil` to use every column in the `SFrame`.

`rows`  

A range of indices; Set to `nil` to use every row in the `SFrame`.

## Discussion

Throws

An `SFrameReadingError` instance.

## See Also

### Creating a Data Frame from Turi Create Types

struct ShapedData

A collection type that represents multidimensional data in a data frame element.

