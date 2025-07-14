

- XCTest
- XCTSourceCodeLocation
-  init(fileURL:lineNumber:) 

Initializer

# init(fileURL:lineNumber:)

Initializes a new instance with a file URL and a line number.

``` source
init(
    fileURL: URL,
    lineNumber: Int
)
```

## Parameters 

`fileURL`  

A file URL that represents the file-system location of the source code file.

`lineNumber`  

An integer that represents a line of code in the source code file.

## See Also

### Initializers

convenience init(filePath: String, lineNumber: Int)

Initializes a new instance with a file path and a line number.

convenience init(filePath: StaticString, lineNumber: UInt)

Initializes a new instance with a file path and a line number.

