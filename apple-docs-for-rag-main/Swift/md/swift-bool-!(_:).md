

- Swift
- Bool
-  !(\_:) 

Operator

# !(\_:)

Performs a logical NOT operation on a Boolean value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func ! (a: Bool) -> Bool
```

## Parameters 

`a`  

The Boolean value to negate.

## Discussion

The logical NOT operator (`!`) inverts a Boolean value. If the value is `true`, the result of the operation is `false`; if the value is `false`, the result is `true`.

```
var printedMessage = false

if !printedMessage {
    print("You look nice today!")
    printedMessage = true
}
// Prints "You look nice today!"
```

## See Also

### Transforming a Boolean

func toggle()

Toggles the Boolean variable’s value.

static func || (Bool, @autoclosure () throws -> Bool) rethrows -> Bool

Performs a logical OR operation on two Boolean values.

static func &amp;&amp; (Bool, @autoclosure () throws -> Bool) rethrows -> Bool

Performs a logical AND operation on two Boolean values.

