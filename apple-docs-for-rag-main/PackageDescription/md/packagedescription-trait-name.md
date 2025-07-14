

- PackageDescription
- Trait
-  name 

Instance Property

# name

The trait’s canonical name.

SwiftPM 6.1+

``` source
var name: String
```

## Discussion

This is used when enabling the trait or when referring to it from other modifiers in the manifest.

The following rules are enforced on trait names:

- The first character must be a Unicode XID start character (most letters), a digit, or `_`.

- Subsequent characters must be a Unicode XID continue character (a digit, `_`, or most letters), `-`, or `+`.

- `default` and `defaults` (in any letter casing combination) are not allowed as trait names to avoid confusion with default traits.

