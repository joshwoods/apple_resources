

- ManagedSettings
- SafariSettings
- SafariSettings.CookiePolicy
-  ...(\_:\_:) 

Operator

# ...(\_:\_:)

Returns a closed range that contains both of its bounds.

ManagedSettingsSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
static func ... (minimum: Self, maximum: Self) -> ClosedRange
```

## Parameters 

`minimum`  

The lower bound for the range.

`maximum`  

The upper bound for the range.

## Discussion

Use the closed range operator (`...`) to create a closed range of any type that conforms to the `Comparable` protocol. This example creates a `ClosedRange` from “a” up to, and including, “z”.

```
let lowercase = "a"..."z"
print(lowercase.contains("z"))
// Prints "true"
```

Precondition

`minimum 

## See Also

### Getting the Range

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func ... (Self) -> PartialRangeThrough&lt;Self>

Returns a partial range up to, and including, its upper bound.

static func ... (Self) -> PartialRangeFrom&lt;Self>

Returns a partial range extending upward from a lower bound.

var hashValue: Int

func hash(into: inout Hasher)

