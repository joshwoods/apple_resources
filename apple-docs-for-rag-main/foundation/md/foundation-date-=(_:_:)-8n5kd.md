

- Foundation
- Date
-  \>=(\_:\_:) 

Operator

# \>=(\_:\_:)

Returns a Boolean value indicating whether the value of the first argument is greater than or equal to that of the second argument.

FoundationSwiftiOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func >= (lhs: Self, rhs: Self) -> Bool
```

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Return Value

`true` if `lhs` is greater than or equal to `rhs`; otherwise, `false`.

## Discussion

This is the default implementation of the greater-than-or-equal-to operator (`>=`) for any type that conforms to `Comparable`.

## See Also

### Comparing Dates

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func > (Date, Date) -> Bool

Returns true if the left hand `Date` is later in time than the right hand `Date`.

static func &lt; (Date, Date) -> Bool

Returns true if the left hand `Date` is earlier in time than the right hand `Date`.

static func &lt;= (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than or equal to that of the second argument.

func compare(Date) -> ComparisonResult

Compares another date to this one.

