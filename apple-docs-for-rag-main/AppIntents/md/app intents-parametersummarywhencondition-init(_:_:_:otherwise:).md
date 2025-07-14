

- App Intents
- ParameterSummaryWhenCondition
-  init(\_:\_:\_:otherwise:) 

Initializer

# init(\_:\_:\_:otherwise:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    _ keyPath: KeyPath,
    _ comparisonOperator: HasValueComparisonOperator,
    @ParameterSummaryBuilder _ when: () -> WhenCondition,
    @ParameterSummaryBuilder otherwise: () -> Otherwise
) where Parameter : AnyIntentValue
```

## See Also

### Creating a conditional statement

enum EquatableComparisonOperator

Operators that indicate the type of equality check for a conditional statement.

enum ComparableComparisonOperator

Operators that indicate the type of comparison check for a conditional statement.

enum HasValueComparisonOperator

Operators that indicate the type of value check for a conditional statement.

enum OneOfComparisonOperator

Operators that indicate the type of containment check for a conditional statement.

