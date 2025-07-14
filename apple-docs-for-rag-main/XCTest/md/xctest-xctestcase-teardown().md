

- XCTest
- XCTestCase
-  tearDown() 

Type Method

# tearDown()

Provides an opportunity to perform cleanup after a test case ends.

``` source
class func tearDown()
```

## Mentioned in 

Set Up and Tear Down State in Your Tests

## Discussion

The tearDown() class method is called exactly once for a test case, after its final test method completes. Override this method to perform any cleanup after all test methods have ended.

## See Also

### Related Documentation

func tearDown()

Provides an opportunity to perform cleanup after each test method in a test case ends.

### Customizing Test Setup and Teardown

Set Up and Tear Down State in Your Tests

Prepare initial state before tests run, and clean up resources after tests complete.

class func setUp()

Provides an opportunity to customize initial state before a test case begins.

func addTeardownBlock(() async throws -> Void)

Registers a block of teardown code to run after the current test method ends.

func addTeardownBlock(() throws -> Void)

Registers a block of teardown code to run after the current test method ends.

