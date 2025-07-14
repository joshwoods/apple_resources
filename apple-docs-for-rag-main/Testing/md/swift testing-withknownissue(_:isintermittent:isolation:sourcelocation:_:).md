

- Swift Testing
-  withKnownIssue(\_:isIntermittent:isolation:sourceLocation:\_:) 

Function

# withKnownIssue(\_:isIntermittent:isolation:sourceLocation:\_:)

Invoke a function that has a known issue that is expected to occur during its execution.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
func withKnownIssue(
    _ comment: Comment? = nil,
    isIntermittent: Bool = false,
    isolation: isolated (any Actor)? = #isolation,
    sourceLocation: SourceLocation = #_sourceLocation,
    _ body: () async throws -> Void
) async
```

## Parameters 

`comment`  

An optional comment describing the known issue.

`isIntermittent`  

Whether or not the known issue occurs intermittently. If this argument is `true` and the known issue does not occur, no secondary issue is recorded.

`isolation`  

The actor to which `body` is isolated, if any.

`sourceLocation`  

The source location to which any recorded issues should be attributed.

`body`  

The function to invoke.

## Mentioned in 

Migrating a test from XCTest

## Discussion

Use this function when a test is known to raise one or more issues that should not cause the test to fail. For example:

```
@Test func example() {
  await withKnownIssue {
    try await flakyCall()
  }
}
```

Because all errors thrown by `body` are caught as known issues, this function is not throwing. If only some errors or issues are known to occur while others should continue to cause test failures, use withKnownIssue(_:isIntermittent:isolation:sourceLocation:_:when:matching:) instead.

## See Also

### Recording known issues in tests

func withKnownIssue(Comment?, isIntermittent: Bool, sourceLocation: SourceLocation, () throws -> Void)

Invoke a function that has a known issue that is expected to occur during its execution.

func withKnownIssue(Comment?, isIntermittent: Bool, sourceLocation: SourceLocation, () throws -> Void, when: () -> Bool, matching: KnownIssueMatcher) rethrows

Invoke a function that has a known issue that is expected to occur during its execution.

func withKnownIssue(Comment?, isIntermittent: Bool, isolation: isolated (any Actor)?, sourceLocation: SourceLocation, () async throws -> Void, when: () async -> Bool, matching: KnownIssueMatcher) async rethrows

Invoke a function that has a known issue that is expected to occur during its execution.

typealias KnownIssueMatcher

A function that is used to match known issues.

