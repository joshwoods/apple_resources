

- XCTest
- XCTest
-  setUp() 

Instance Method

# setUp()

Provides an opportunity to reset state before calling each test method in a test case.

``` source
func setUp()
```

## Mentioned in 

Set Up and Tear Down State in Your Tests

## Discussion

Before each test begins, `XCTest` calls setUp(completion:) for asynchronous state preparation, then \`\`XCTest/XCTest/setUpWithError()\`\`\`,\` followed by this method. Override this method to reset state for each test method.

If state preparation might throw errors, override setUp(completion:) or setUpWithError() instead.

## See Also

### Related Documentation

class func setUp()

Provides an opportunity to customize initial state before a test case begins.

Set Up and Tear Down State in Your Tests

Prepare initial state before tests run, and clean up resources after tests complete.

### Setting Up and Tearing Down

func setUp(completion: ((any Error)?) -> Void)

Provides an opportunity to reset state asynchronously and handle errors before calling each test method in a test case.

func setUpWithError() throws

Provides an opportunity to reset state and to throw errors before calling each test method in a test case.

func tearDown(completion: ((any Error)?) -> Void)

Provides an opportunity to perform cleanup asynchronously and handle errors after each test method in a test case ends.

func tearDownWithError() throws

Provides an opportunity to perform cleanup and to throw errors after each test method in a test case ends.

func tearDown()

Provides an opportunity to perform cleanup after each test method in a test case ends.

