

- Swift Testing
- Traits
- TimeLimitTrait
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

### Type Methods

static func timeLimit(TimeLimitTrait.Duration) -> Self

Construct a time limit trait that causes a test to time out if it runs for too long.

