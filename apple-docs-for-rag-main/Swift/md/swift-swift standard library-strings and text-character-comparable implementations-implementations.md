

- Swift
- Swift Standard Library
- Strings and Text
- Character
-  Comparable Implementations 

API Collection

# Comparable Implementations

## Topics

### Operators

static func ... (Self) -> PartialRangeThrough&lt;Self>

Returns a partial range up to, and including, its upper bound.

static func ... (Self) -> PartialRangeFrom&lt;Self>

Returns a partial range extending upward from a lower bound.

static func ... (Self, Self) -> ClosedRange&lt;Self>

Returns a closed range that contains both of its bounds.

static func ..&lt; (Self) -> PartialRangeUpTo&lt;Self>

Returns a partial range up to, but not including, its upper bound.

static func ..&lt; (Self, Self) -> Range&lt;Self>

Returns a half-open range that contains its lower bound but not its upper bound.

static func &lt; (Character, Character) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

static func > (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is greater than that of the second argument.

static func &lt;= (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than or equal to that of the second argument.

static func >= (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is greater than or equal to that of the second argument.

