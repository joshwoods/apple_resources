

- AVFoundation
- AVCaptureIndexPicker
-  init(\_:symbolName:localizedIndexTitles:) 

Initializer

# init(\_:symbolName:localizedIndexTitles:)

Creates an object to select an index from a set of values.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
init(
    _ localizedTitle: String,
    symbolName: String,
    localizedIndexTitles: [String]
)
```

## Parameters 

`localizedTitle`  

A localized title that describes the control’s action.

`symbolName`  

The name of an SF Symbol that represents the control.

`localizedIndexTitles`  

The titles to use for each index. The array must not be empty.

## Discussion

Create a picker with this initializer when you already have an array containing a title for each picked value.

## See Also

### Creating an index picker

init(String, symbolName: String, numberOfIndexes: Int)

Creates a control to pick a value from the specified number of indexes.

init(String, symbolName: String, numberOfIndexes: Int, localizedTitleTransform: (Int) -> String)

Creates a control to pick a value from the specified number of indices.

