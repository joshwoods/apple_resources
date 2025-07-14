

- Foundation
- PredicateExpressions
-  build_ClosedRange(lower:upper:) 

Type Method

# build_ClosedRange(lower:upper:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func build_ClosedRange(
    lower: LHS,
    upper: RHS
) -> PredicateExpressions.ClosedRange where LHS : PredicateExpression, RHS : PredicateExpression, LHS.Output : Comparable, LHS.Output == RHS.Output
```

