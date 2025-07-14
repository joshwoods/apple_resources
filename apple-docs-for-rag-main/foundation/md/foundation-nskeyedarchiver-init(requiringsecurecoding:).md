

- Foundation
- NSKeyedArchiver
-  init(requiringSecureCoding:) 

Initializer

# init(requiringSecureCoding:)

Creates an archiver to encode data, and optionally disables secure coding.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
init(requiringSecureCoding requiresSecureCoding: Bool)
```

## Parameters 

`requiresSecureCoding`  

A Boolean value indicating whether all encoded objects must conform to NSSecureCoding.

## Discussion

To prevent the possibility of encoding an object that NSKeyedUnarchiver can’t decode, set `requiresSecureCoding` to true whenever possible. This ensures that all encoded objects conform to NSSecureCoding.

Note

Enabling secure coding doesn’t change the output format of the archive. This means that you can encode archives with secure coding enabled, and decode them later with secure coding disabled.

## See Also

### Related Documentation

var requiresSecureCoding: Bool

Indicates whether the archiver requires all archived classes to resist object substitution attacks.

### Creating a Keyed Archiver

init()

Initializes an archiver to encode data.

Deprecated

init(forWritingWith: NSMutableData)

Initializes an archiver to encode data into a given a mutable-data object.

Deprecated

