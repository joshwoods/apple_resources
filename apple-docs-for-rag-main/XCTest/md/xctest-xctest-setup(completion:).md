

- XCTest
- XCTest
-  setUp(completion:) 

Instance Method

# setUp(completion:)

Provides an opportunity to reset state asynchronously and handle errors before calling each test method in a test case.

``` source
func setUp(completion: @escaping ((any Error)?) -> Void)
```

``` source
func setUp() async throws
```

## Parameters 

`completion`  

In Swift, reserved for system usage. Do not use. In Objective-C, a completion block you must call after you have completed setting up your state asynchronously.

## Mentioned in 

Set Up and Tear Down State in Your Tests

## Discussion

Concurrency Note

In Swift, `XCTest` does not support overriding this method with a completion handler. Override this method for asynchronous test setup with the following declaration:

```
func setUp() async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

In Swift, override `setUp() async throws` for asynchronous state preparation with error handling before each test. Do not override `setUp(completion:)` for synchronous state preparation. In Objective-C, override this method for asynchronous state preparation with error handling before each test. Call the completion handler after you have set up your state to notify the test system it can proceed with the next task.

Before each test begins, `XCTest` calls:

1.  This method for asynchronous state preparation and error handling,

2.  setUpWithError() for synchronous state preparation and error handling,

3.  Then setUp() for synchronous state preparation without error handling.

For setup methods that provide error handling, `XCTest` marks the test failed when it catches errors, or skipped when it catches XCTSkip. Based on your state preparation requirements, choose one of these methods to override in your test case.

## See Also

### Setting Up and Tearing Down

func setUpWithError() throws

Provides an opportunity to reset state and to throw errors before calling each test method in a test case.

func setUp()

Provides an opportunity to reset state before calling each test method in a test case.

func tearDown(completion: ((any Error)?) -> Void)

Provides an opportunity to perform cleanup asynchronously and handle errors after each test method in a test case ends.

func tearDownWithError() throws

Provides an opportunity to perform cleanup and to throw errors after each test method in a test case ends.

func tearDown()

Provides an opportunity to perform cleanup after each test method in a test case ends.

