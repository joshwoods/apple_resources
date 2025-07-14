

- XCTest
- XCTestCase
-  setUp() 

Type Method

# setUp()

Provides an opportunity to customize initial state before a test case begins.

``` source
class func setUp()
```

## Mentioned in 

Set Up and Tear Down State in Your Tests

## Discussion

The setUp() class method is called exactly once for a test case, before its first test method is called. Override this method to customize the initial state for all tests in the test case.

## See Also

### Related Documentation

func setUp()

Provides an opportunity to reset state before calling each test method in a test case.

### Customizing Test Setup and Teardown

Set Up and Tear Down State in Your Tests

Prepare initial state before tests run, and clean up resources after tests complete.

func addTeardownBlock(() async throws -> Void)

Registers a block of teardown code to run after the current test method ends.

func addTeardownBlock(() throws -> Void)

Registers a block of teardown code to run after the current test method ends.

class func tearDown()

Provides an opportunity to perform cleanup after a test case ends.

