

- XCTest
- XCTNSPredicateExpectation
-  XCTNSPredicateExpectation.Handler 

Type Alias

# XCTNSPredicateExpectation.Handler

A handler XCTest calls when evaluating the predicate returns `true`.

``` source
typealias Handler = () -> Bool
```

## Return Value

Your custom handler should return true if the expectation is considered fulfilled, otherwise false.

## See Also

### Handling Predicate Resolution

var handler: XCTNSPredicateExpectation.Handler?

An optional handler that performs custom evaluation when `predicate` evaluates as `true`.

