

- Swift Testing
- SourceLocation
-  init(fileID:filePath:line:column:) 

Initializer

# init(fileID:filePath:line:column:)

Initialize an instance of this type with the specified location details.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
init(
    fileID: String,
    filePath: String,
    line: Int,
    column: Int
)
```

## Parameters 

`fileID`  

The file ID of the source file, using the format described in the documentation for the #fileID macro in the Swift standard library.

`filePath`  

The path to the source file.

`line`  

The line in the source file. Must be greater than `0`.

`column`  

The column in the source file. Must be greater than `0`.

## Discussion

Precondition

`fileID` must not be empty and must be formatted as described in the documentation for #fileID.

Precondition

`line` must be greater than `0`.

Precondition

`column` must be greater than `0`.

