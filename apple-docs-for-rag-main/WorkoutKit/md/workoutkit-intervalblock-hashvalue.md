

- WorkoutKit
- IntervalBlock
-  hashValue 

Instance Property

# hashValue

The hashed value of the interval block.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
var hashValue: Int { get }
```

## See Also

### Hashing interval blocks

func hash(into: inout Hasher)

Hashes the essential components of the interval block by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two interval blocks aren’t equal.

static func == (IntervalBlock, IntervalBlock) -> Bool

Returns a Boolean value that indicates whether two interval blocks are equal.

