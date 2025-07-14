

- XCTest
- XCTSourceCodeContext
-  init(location:) 

Initializer

# init(location:)

Initializes a new instance with a call stack from the executing thread and a provided source code location.

``` source
convenience init(location: XCTSourceCodeLocation?)
```

## Parameters 

`location`  

A representation of a location in source code.

## Discussion

The system derives the call stack from `NSThread.callStackReturnAddresses.`

## See Also

### Initializers

init(callStack: [XCTSourceCodeFrame], location: XCTSourceCodeLocation?)

Initializes a new instance with a provided call stack and source code location.

convenience init(callStackAddresses: [NSNumber], location: XCTSourceCodeLocation?)

Initializes a new instance with an array of call stack addresses and a source code location.

convenience init()

Initializes a new instance with a call stack from the executing thread and no location.

