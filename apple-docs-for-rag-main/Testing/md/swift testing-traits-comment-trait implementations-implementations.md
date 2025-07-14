

- Swift Testing
- Traits
- Comment
-  Trait Implementations 

API Collection

# Trait Implementations

## Topics

### Instance Properties

var comments: [Comment]

The user-provided comments for this trait, if any.

### Instance Methods

func prepare(for: Test) async throws

Prepare to run the test to which this trait was added.

func scopeProvider(for: Test, testCase: Test.Case?) -> Never?

Get this trait’s scope provider for the specified test and/or test case, if any.

### Type Aliases

typealias TestScopeProvider

The type of the test scope provider for this trait.

