

- XCTest
- XCTSourceCodeLocation
-  init(filePath:lineNumber:) 

Initializer

# init(filePath:lineNumber:)

Initializes a new instance with a file path and a line number.

``` source
convenience init(
    filePath: StaticString = #filePath,
    lineNumber: UInt = #line
)
```

## Parameters 

`filePath`  

A string that represents a file path to the source code file.

`lineNumber`  

An integer that represents a line of code in the source code file.

## See Also

### Initializers

init(fileURL: URL, lineNumber: Int)

Initializes a new instance with a file URL and a line number.

convenience init(filePath: String, lineNumber: Int)

Initializes a new instance with a file path and a line number.

