

- Swift
- Swift Standard Library
- Debugging and Reflection
- Never
-  TestScoping Implementations 

API Collection

# TestScoping Implementations

## Topics

### Instance Methods

func provideScope(for: Test, testCase: Test.Case?, performing: () async throws -> Void) async throws

Provide custom execution scope for a function call which is related to the specified test or test case.

