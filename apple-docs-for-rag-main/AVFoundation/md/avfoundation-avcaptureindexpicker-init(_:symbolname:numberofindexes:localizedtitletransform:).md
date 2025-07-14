

- AVFoundation
- AVCaptureIndexPicker
-  init(\_:symbolName:numberOfIndexes:localizedTitleTransform:) 

Initializer

# init(\_:symbolName:numberOfIndexes:localizedTitleTransform:)

Creates a control to pick a value from the specified number of indices.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
init(
    _ localizedTitle: String,
    symbolName: String,
    numberOfIndexes: Int,
    localizedTitleTransform: (Int) -> String
)
```

## Parameters 

`localizedTitle`  

A localized title that describes the picker’s action.

`symbolName`  

The name of the symbol from the SF Symbols library to use to represent this control.

`numberOfIndexes`  

The number of indexes to pick between. This value must be greater than `0`.

`localizedTitleTransform`  

A transformation from index to localized title.

## Discussion

Create a picker with this initializer if your app requires specifying a title for each value lazily.

## See Also

### Creating an index picker

init(String, symbolName: String, numberOfIndexes: Int)

Creates a control to pick a value from the specified number of indexes.

init(String, symbolName: String, localizedIndexTitles: [String])

Creates an object to select an index from a set of values.

