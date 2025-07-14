

- WorkoutKit
- IntervalBlock
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value that indicates whether two interval blocks are equal.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
static func == (a: IntervalBlock, b: IntervalBlock) -> Bool
```

## See Also

### Hashing interval blocks

var hashValue: Int

The hashed value of the interval block.

func hash(into: inout Hasher)

Hashes the essential components of the interval block by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two interval blocks aren’t equal.

