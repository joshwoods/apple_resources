

- RealityKit
- ARView
- 
  - ARView
- ARView.Environment
- ARView.Environment.Reverb
- ARView.Environment.Reverb.Preset
-  hashValue 

Instance Property

# hashValue

The hash value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
var hashValue: Int { get }
```

## Discussion

Hash values are not guaranteed to be equal across different executions of your program. Do not save hash values to use during a future execution.

Important

`hashValue` is deprecated as a `Hashable` requirement. To conform to `Hashable`, implement the `hash(into:)` requirement instead. The compiler provides an implementation for `hashValue` for you.

## See Also

### Comparing reverb presets

static func == (ARView.Environment.Reverb.Preset, ARView.Environment.Reverb.Preset) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

