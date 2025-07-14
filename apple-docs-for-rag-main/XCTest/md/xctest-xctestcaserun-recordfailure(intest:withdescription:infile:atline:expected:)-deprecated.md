

- XCTest
- XCTestCaseRun
-  recordFailure(inTest:withDescription:inFile:atLine:expected:) Deprecated

Instance Method

# recordFailure(inTest:withDescription:inFile:atLine:expected:)

Records a test failure during test execution for this test run.

``` source
func recordFailure(
    inTest testCase: XCTestCase,
    withDescription description: String,
    inFile filePath: String,
    atLine lineNumber: Int,
    expected: Bool
)
```

Deprecated

Use record(_:) instead.

