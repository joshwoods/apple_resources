

- XCTest
- XCTExpectedFailure
-  issue 

Instance Property

# issue

The issue that fulfills the expected failure.

**macOS**

``` source
@NSCopying
var issue: XCTIssueReference { get }
```

**iOS, iPadOS, tvOS, visionOS, watchOS**

``` source
var issue: XCTIssue { get }
```

## See Also

### Detailing Expected Failure

var failureReason: String?

An optional string that describes why the test expects a failure.

