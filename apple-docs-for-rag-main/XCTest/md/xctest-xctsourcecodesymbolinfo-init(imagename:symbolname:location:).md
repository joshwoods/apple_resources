

- XCTest
- XCTSourceCodeSymbolInfo
-  init(imageName:symbolName:location:) 

Initializer

# init(imageName:symbolName:location:)

Initializes an instance with a binary image name, source code location, and symbol name.

``` source
init(
    imageName: String,
    symbolName: String,
    location: XCTSourceCodeLocation?
)
```

## Parameters 

`imageName`  

A string that represents the name of the binary image containing the symbolicated code.

`symbolName`  

A string that represents a human-readable symbol in source code.

`location`  

A representation of a location in source code.

