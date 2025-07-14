

- XCTest
- XCTestExpectation
-  fulfill() 

Instance Method

# fulfill()

Marks the expectation as having been met.

``` source
func fulfill()
```

## Discussion

It is an error to call this method on an expectation that has already been fulfilled, or when the test case that vended the expectation has already completed.

