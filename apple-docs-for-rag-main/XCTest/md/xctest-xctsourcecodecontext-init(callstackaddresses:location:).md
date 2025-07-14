

- XCTest
- XCTSourceCodeContext
-  init(callStackAddresses:location:) 

Initializer

# init(callStackAddresses:location:)

Initializes a new instance with an array of call stack addresses and a source code location.

``` source
convenience init(
    callStackAddresses: [NSNumber],
    location: XCTSourceCodeLocation?
)
```

## Parameters 

`callStackAddresses`  

An array of call stack return addresses.

`location`  

A representation of a location in source code.

## Discussion

The call stack addresses could be from `NSThread.callStackReturnAddresses`, `NSException.callStackReturnAddresses`, or another source.

## See Also

### Initializers

init(callStack: [XCTSourceCodeFrame], location: XCTSourceCodeLocation?)

Initializes a new instance with a provided call stack and source code location.

convenience init(location: XCTSourceCodeLocation?)

Initializes a new instance with a call stack from the executing thread and a provided source code location.

convenience init()

Initializes a new instance with a call stack from the executing thread and no location.

