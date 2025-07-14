

- XCTest
- XCTKVOExpectation
-  XCTKVOExpectation.Handler 

Type Alias

# XCTKVOExpectation.Handler

A custom handler to call when observing a KVO change for a specified key path.

``` source
typealias Handler = (Any, [AnyHashable : Any]) -> Bool
```

## Parameters 

`observedObject`  

The observed object, which helps to avoid block-capture issues.

`change`  

The KVO change dictionary.

## Return Value

Your custom handler returns true if the system fulfills the expectation after the observed change; otherwise, false.

## See Also

### Custom KVO evaluation

var handler: XCTKVOExpectation.Handler?

An optional handler that performs custom evaluation of changes to the observed key path.

