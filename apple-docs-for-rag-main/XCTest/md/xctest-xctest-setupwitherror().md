

- XCTest
- XCTest
-  setUpWithError() 

Instance Method

# setUpWithError()

Provides an opportunity to reset state and to throw errors before calling each test method in a test case.

``` source
func setUpWithError() throws
```

## Mentioned in 

Set Up and Tear Down State in Your Tests

## Discussion

Before each test begins, `XCTest` calls setUp(completion:) for asynchronous state preparation, then this method, followed by setUp().

If state preparation might throw errors, override setUp(completion:) or this method. `XCTest` marks the test failed when it catches errors, or skipped when it catches `XCTSkip`.

## See Also

### Setting Up and Tearing Down

func setUp(completion: ((any Error)?) -> Void)

Provides an opportunity to reset state asynchronously and handle errors before calling each test method in a test case.

func setUp()

Provides an opportunity to reset state before calling each test method in a test case.

func tearDown(completion: ((any Error)?) -> Void)

Provides an opportunity to perform cleanup asynchronously and handle errors after each test method in a test case ends.

func tearDownWithError() throws

Provides an opportunity to perform cleanup and to throw errors after each test method in a test case ends.

func tearDown()

Provides an opportunity to perform cleanup after each test method in a test case ends.

