

- Swift Testing
-  KnownIssueMatcher 

Type Alias

# KnownIssueMatcher

A function that is used to match known issues.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
typealias KnownIssueMatcher = (Issue) -> Bool
```

## Parameters 

`issue`  

The issue to match.

## Return Value

Whether or not `issue` is known to occur.

## See Also

### Recording known issues in tests

func withKnownIssue(Comment?, isIntermittent: Bool, sourceLocation: SourceLocation, () throws -> Void)

Invoke a function that has a known issue that is expected to occur during its execution.

func withKnownIssue(Comment?, isIntermittent: Bool, isolation: isolated (any Actor)?, sourceLocation: SourceLocation, () async throws -> Void) async

Invoke a function that has a known issue that is expected to occur during its execution.

func withKnownIssue(Comment?, isIntermittent: Bool, sourceLocation: SourceLocation, () throws -> Void, when: () -> Bool, matching: KnownIssueMatcher) rethrows

Invoke a function that has a known issue that is expected to occur during its execution.

func withKnownIssue(Comment?, isIntermittent: Bool, isolation: isolated (any Actor)?, sourceLocation: SourceLocation, () async throws -> Void, when: () async -> Bool, matching: KnownIssueMatcher) async rethrows

Invoke a function that has a known issue that is expected to occur during its execution.

