

- XCTest
- XCTestCase
-  addTeardownBlock(\_:) 

Instance Method

# addTeardownBlock(\_:)

Registers a block of teardown code to run after the current test method ends.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
@preconcurrency
func addTeardownBlock(_ block: @escaping @MainActor () throws -> Void)
```

## Parameters 

`block`  

A block of teardown code.

## See Also

### Customizing Test Setup and Teardown

Set Up and Tear Down State in Your Tests

Prepare initial state before tests run, and clean up resources after tests complete.

class func setUp()

Provides an opportunity to customize initial state before a test case begins.

func addTeardownBlock(() async throws -> Void)

Registers a block of teardown code to run after the current test method ends.

class func tearDown()

Provides an opportunity to perform cleanup after a test case ends.

