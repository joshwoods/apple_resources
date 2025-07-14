

- Foundation
- NSPointerFunctions
- NSPointerFunctions.Options
-  structPersonality 

Type Property

# structPersonality

Use a memory hash and `memcmp` (using a size function that you must set—see sizeFunction).

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var structPersonality: NSPointerFunctions.Options { get }
```

## See Also

### Personality Options

static var cStringPersonality: NSPointerFunctions.Options

Use a string hash and `strcmp`; C-string ‘`%s`’ style description.

static var integerPersonality: NSPointerFunctions.Options

Use unshifted value as hash and equality.

static var objectPersonality: NSPointerFunctions.Options

Use `hash` and `isEqual` methods for hashing and equality comparisons, use the `description` method for a description.

static var objectPointerPersonality: NSPointerFunctions.Options

Use shifted pointer for the hash value and direct comparison to determine equality; use the `description` method for a description.

static var opaquePersonality: NSPointerFunctions.Options

Use shifted pointer for the hash value and direct comparison to determine equality.

static var cStringPersonality: NSPointerFunctions.Options

Use a string hash and `strcmp`; C-string ‘`%s`’ style description.

static var integerPersonality: NSPointerFunctions.Options

Use unshifted value as hash and equality.

static var objectPersonality: NSPointerFunctions.Options

Use `hash` and `isEqual` methods for hashing and equality comparisons, use the `description` method for a description.

static var objectPointerPersonality: NSPointerFunctions.Options

Use shifted pointer for the hash value and direct comparison to determine equality; use the `description` method for a description.

static var opaquePersonality: NSPointerFunctions.Options

Use shifted pointer for the hash value and direct comparison to determine equality.

let NSMapTableObjectPointerPersonality: NSPointerFunctions.Options

Equivalent to objectPointerPersonality.

