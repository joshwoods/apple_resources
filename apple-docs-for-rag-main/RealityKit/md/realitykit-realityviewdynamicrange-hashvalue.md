

- RealityKit
- RealityViewDynamicRange
-  hashValue 

Instance Property

# hashValue

The hash value.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
var hashValue: Int { get }
```

## Discussion

Hash values are not guaranteed to be equal across different executions of your program. Do not save hash values to use during a future execution.

Important

`hashValue` is deprecated as a `Hashable` requirement. To conform to `Hashable`, implement the `hash(into:)` requirement instead. The compiler provides an implementation for `hashValue` for you.

## See Also

### Protocol support

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

static func == (RealityViewDynamicRange, RealityViewDynamicRange) -> Bool

Returns a Boolean value indicating whether two values are equal.

