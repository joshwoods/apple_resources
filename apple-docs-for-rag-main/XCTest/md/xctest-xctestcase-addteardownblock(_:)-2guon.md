

- XCTest
- XCTestCase
-  addTeardownBlock(\_:) 

Instance Method

# addTeardownBlock(\_:)

Registers a block of teardown code to run after the current test method ends.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
func addTeardownBlock(_ block: @escaping () async throws -> Void)
```

## Parameters 

`block`  

A block of code that cleans up resources after a test run.

## Discussion

Call this method during a test method’s execution to register a block of code to be called when the test method ends. The block of code may contain asynchronous teardown logic; the test system waits until the asynchronous teardown is complete before proceeding.

Registered teardown blocks are called before the tearDown(), tearDownWithError(), or tearDown(completion:) instance methods for their associated test case are executed. Teardown blocks are run on the main thread, but can be registered from any thread. Each registered block is run once, in last-in, first-out order, executed serially.

Note

You can register a teardown block within a test case’s setUp(), setUpWithError(), or setUp(completion:) instance methods, but not from within its tearDown(), tearDownWithError(), or tearDown(completion:) instance methods, or from within another teardown block. Teardown blocks always execute before the test system calls the tearDown(), tearDownWithError(), or tearDown(completion:) instance methods.

Use teardown blocks to write test-specific teardown code alongside associated setup code. For example, if a test method needs to create a resource that must be deleted when the test completes, write the code to create the resource, followed immediately by code that registers a teardown block to delete the resource.

## See Also

### Customizing Test Setup and Teardown

Set Up and Tear Down State in Your Tests

Prepare initial state before tests run, and clean up resources after tests complete.

class func setUp()

Provides an opportunity to customize initial state before a test case begins.

func addTeardownBlock(() throws -> Void)

Registers a block of teardown code to run after the current test method ends.

class func tearDown()

Provides an opportunity to perform cleanup after a test case ends.

