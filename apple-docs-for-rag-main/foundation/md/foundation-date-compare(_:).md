

- Foundation
- Date
-  compare(\_:) 

Instance Method

# compare(\_:)

Compares another date to this one.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func compare(_ other: Date) -> ComparisonResult
```

## Parameters 

`other`  

Another date.

## See Also

### Comparing Dates

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func > (Date, Date) -> Bool

Returns true if the left hand `Date` is later in time than the right hand `Date`.

static func >= (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is greater than or equal to that of the second argument.

static func &lt; (Date, Date) -> Bool

Returns true if the left hand `Date` is earlier in time than the right hand `Date`.

static func &lt;= (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than or equal to that of the second argument.

