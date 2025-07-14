

- XCTest
- XCTIssueReference
-  detailedDescription 

Instance Property

# detailedDescription

A detailed description of the issue that may include transient data, such as numbers, object identifiers, and timestamps, to help diagnose the issue.

``` source
var detailedDescription: String? { get }
```

## See Also

### Issue Details

var type: XCTIssueReference.IssueType

A value for classifying an issue that occurs during testing.

var compactDescription: String

A concise description of the issue with no transient data, suitable for use in test run summaries and results aggregation across multiple test runs.

var sourceCodeContext: XCTSourceCodeContext

The source code location for the issue, including the filename, line number, and call stack.

var associatedError: (any Error)?

An optional error to associate with a test issue.

var attachments: [XCTAttachment]

An array of data that augments a test issue, such as files, images, screenshots, data blobs, or ZIP files.

