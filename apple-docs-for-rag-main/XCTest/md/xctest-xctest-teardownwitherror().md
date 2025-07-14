

- XCTest
- XCTest
-  tearDownWithError() 

Instance Method

# tearDownWithError()

Provides an opportunity to perform cleanup and to throw errors after each test method in a test case ends.

``` source
func tearDownWithError() throws
```

## Discussion

After each test completes, `XCTest` calls tearDown(), then `tearDownWithError()`, followed by tearDown(completion:).

If state cleanup might throw errors, override this method or tearDown(completion:). `XCTest` marks the test failed when it catches errors, or skipped when it catches `XCTSkip`.

## See Also

### Setting Up and Tearing Down

func setUp(completion: ((any Error)?) -> Void)

Provides an opportunity to reset state asynchronously and handle errors before calling each test method in a test case.

func setUpWithError() throws

Provides an opportunity to reset state and to throw errors before calling each test method in a test case.

func setUp()

Provides an opportunity to reset state before calling each test method in a test case.

func tearDown(completion: ((any Error)?) -> Void)

Provides an opportunity to perform cleanup asynchronously and handle errors after each test method in a test case ends.

func tearDown()

Provides an opportunity to perform cleanup after each test method in a test case ends.

