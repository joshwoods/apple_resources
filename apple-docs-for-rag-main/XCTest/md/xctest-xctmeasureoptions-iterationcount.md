

- XCTest
- XCTMeasureOptions
-  iterationCount 

Instance Property

# iterationCount

The number of times the performance test measures its block.

``` source
var iterationCount: Int { get set }
```

## Discussion

A performance test runs its block `iterationCount+1` times, ignoring the first iteration and recording metrics for the remaining iterations. The test ignores the first iteration to reduce measurement variance associated with “warming up” caches and other first-run behavior.

## See Also

### Using Option Details

var invocationOptions: XCTMeasureOptions.InvocationOptions

Options that define whether measurement is automatically or manually controlled.

struct InvocationOptions

Test measurement options that control how measurement starts and stops.

