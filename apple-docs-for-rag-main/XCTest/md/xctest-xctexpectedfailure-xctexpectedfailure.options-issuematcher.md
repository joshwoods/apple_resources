

- XCTest
- XCTExpectedFailure
- XCTExpectedFailure.Options
-  issueMatcher 

Instance Property

# issueMatcher

A block of code that determines whether the test issue fulfills the expected failure.

**iOS, iPadOS, tvOS, visionOS, watchOS**

``` source
var issueMatcher: (XCTIssue) -> Bool { get set }
```

**macOS**

``` source
var issueMatcher: (XCTIssueReference) -> Bool { get set }
```

## Discussion

Provide code to examine the issue and respond with a Boolean value indicating whether the issue fulfills the expected failure.

