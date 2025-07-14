

- RealityKit
- EnvironmentResource
- EnvironmentResource.CreateOptions
- EnvironmentResource.CreateOptions.SamplingQuality
-  hashValue 

Instance Property

# hashValue

The hash value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var hashValue: Int { get }
```

## Discussion

Hash values are not guaranteed to be equal across different executions of your program. Do not save hash values to use during a future execution.

Important

`hashValue` is deprecated as a `Hashable` requirement. To conform to `Hashable`, implement the `hash(into:)` requirement instead. The compiler provides an implementation for `hashValue` for you.

## See Also

### Comparing sampling quality

static func == (EnvironmentResource.CreateOptions.SamplingQuality, EnvironmentResource.CreateOptions.SamplingQuality) -> Bool

Returns a Boolean value indicating whether two values are equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

