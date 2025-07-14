

- Swift
- Bool
-  toggle() 

Instance Method

# toggle()

Toggles the Boolean variable’s value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func toggle()
```

## Discussion

Use this method to toggle a Boolean value from `true` to `false` or from `false` to `true`.

```
var bools = [true, false]

bools[0].toggle()
// bools == [false, false]
```

## See Also

### Transforming a Boolean

static func ! (Bool) -> Bool

Performs a logical NOT operation on a Boolean value.

static func || (Bool, @autoclosure () throws -> Bool) rethrows -> Bool

Performs a logical OR operation on two Boolean values.

static func &amp;&amp; (Bool, @autoclosure () throws -> Bool) rethrows -> Bool

Performs a logical AND operation on two Boolean values.

