

- XCTest
- XCTSourceCodeContext
-  init(callStack:location:) 

Initializer

# init(callStack:location:)

Initializes a new instance with a provided call stack and source code location.

``` source
init(
    callStack: [XCTSourceCodeFrame],
    location: XCTSourceCodeLocation?
)
```

## Parameters 

`callStack`  

An array of source code frames that describe the call stack.

`location`  

A representation of a location in source code.

## See Also

### Initializers

convenience init(callStackAddresses: [NSNumber], location: XCTSourceCodeLocation?)

Initializes a new instance with an array of call stack addresses and a source code location.

convenience init(location: XCTSourceCodeLocation?)

Initializes a new instance with a call stack from the executing thread and a provided source code location.

convenience init()

Initializes a new instance with a call stack from the executing thread and no location.

