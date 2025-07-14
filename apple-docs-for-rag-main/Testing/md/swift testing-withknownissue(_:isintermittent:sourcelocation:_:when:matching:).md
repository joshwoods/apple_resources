

- Swift Testing
-  withKnownIssue(\_:isIntermittent:sourceLocation:\_:when:matching:) 

Function

# withKnownIssue(\_:isIntermittent:sourceLocation:\_:when:matching:)

Invoke a function that has a known issue that is expected to occur during its execution.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
func withKnownIssue(
    _ comment: Comment? = nil,
    isIntermittent: Bool = false,
    sourceLocation: SourceLocation = #_sourceLocation,
    _ body: () throws -> Void,
    when precondition: () -> Bool = { true },
    matching issueMatcher: @escaping KnownIssueMatcher = { _ in true }
) rethrows
```

## Parameters 

`comment`  

An optional comment describing the known issue.

`isIntermittent`  

Whether or not the known issue occurs intermittently. If this argument is `true` and the known issue does not occur, no secondary issue is recorded.

`sourceLocation`  

The source location to which any recorded issues should be attributed.

`body`  

The function to invoke.

`precondition`  

A function that determines if issues are known to occur during the execution of `body`. If this function returns `true`, encountered issues that are matched by `issueMatcher` are considered to be known issues; if this function returns `false`, `issueMatcher` is not called and they are treated as unknown.

`issueMatcher`  

A function to invoke when an issue occurs that is used to determine if the issue is known to occur. By default, all issues match.

## Mentioned in 

Migrating a test from XCTest

## Discussion

Throws

Whatever is thrown by `body`, unless it is matched by `issueMatcher`.

Use this function when a test is known to raise one or more issues that should not cause the test to fail, or if a precondition affects whether issues are known to occur. For example:

```
@Test func example() throws {
  try withKnownIssue {
    try flakyCall()
  } when: {
    callsAreFlakyOnThisPlatform()
  } matching: { issue in
    issue.error is FileNotFoundError
  }
}
```

It is not necessary to specify both `precondition` and `issueMatcher` if only one is relevant. If all errors and issues should be considered known issues, use withKnownIssue(_:isIntermittent:sourceLocation:_:) instead.

Note

`issueMatcher` may be invoked more than once for the same issue.

## See Also

### Recording known issues in tests

func withKnownIssue(Comment?, isIntermittent: Bool, sourceLocation: SourceLocation, () throws -> Void)

Invoke a function that has a known issue that is expected to occur during its execution.

func withKnownIssue(Comment?, isIntermittent: Bool, isolation: isolated (any Actor)?, sourceLocation: SourceLocation, () async throws -> Void) async

Invoke a function that has a known issue that is expected to occur during its execution.

func withKnownIssue(Comment?, isIntermittent: Bool, isolation: isolated (any Actor)?, sourceLocation: SourceLocation, () async throws -> Void, when: () async -> Bool, matching: KnownIssueMatcher) async rethrows

Invoke a function that has a known issue that is expected to occur during its execution.

typealias KnownIssueMatcher

A function that is used to match known issues.

