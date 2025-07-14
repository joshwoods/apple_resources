

- WorkoutKit
- IntervalBlock
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of the interval block by feeding them into the given hash function.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
func hash(into hasher: inout Hasher)
```

## See Also

### Hashing interval blocks

var hashValue: Int

The hashed value of the interval block.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two interval blocks aren’t equal.

static func == (IntervalBlock, IntervalBlock) -> Bool

Returns a Boolean value that indicates whether two interval blocks are equal.

