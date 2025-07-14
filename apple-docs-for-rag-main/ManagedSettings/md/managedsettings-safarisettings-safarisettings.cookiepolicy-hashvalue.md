

- ManagedSettings
- SafariSettings
- SafariSettings.CookiePolicy
-  hashValue 

Instance Property

# hashValue

ManagedSettingsSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
var hashValue: Int { get }
```

Available when `Self` conforms to `Hashable` and `RawValue` conforms to `Hashable`.

## See Also

### Getting the Range

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func ... (Self) -> PartialRangeThrough&lt;Self>

Returns a partial range up to, and including, its upper bound.

static func ... (Self) -> PartialRangeFrom&lt;Self>

Returns a partial range extending upward from a lower bound.

static func ... (Self, Self) -> ClosedRange&lt;Self>

Returns a closed range that contains both of its bounds.

func hash(into: inout Hasher)

