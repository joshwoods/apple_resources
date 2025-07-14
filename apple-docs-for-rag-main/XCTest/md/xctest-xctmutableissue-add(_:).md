

- XCTest
- XCTMutableIssue
-  add(\_:) 

Instance Method

# add(\_:)

Adds supporting data to an issue.

``` source
func add(_ attachment: XCTAttachment)
```

## Parameters 

`attachment`  

A data item that augments an issue, such as a file, image, screenshot, data blob, or ZIP file.

## See Also

### Issue Details

var type: XCTIssueReference.IssueType

A value for classifying an issue that occurs during testing.

var compactDescription: String

A concise description of the issue with no transient data, suitable for use in test run summaries and results aggregation across multiple test runs.

var detailedDescription: String?

A detailed description of the issue that may include transient data, such as numbers, object identifiers, and timestamps, to help diagnose the issue.

var sourceCodeContext: XCTSourceCodeContext

The source code location for the issue, including the filename, line number, and call stack.

var associatedError: (any Error)?

An optional error to associate with a test issue.

var attachments: [XCTAttachment]

An array of data that augments an issue, such as files, images, screenshots, data blobs, or ZIP files.

