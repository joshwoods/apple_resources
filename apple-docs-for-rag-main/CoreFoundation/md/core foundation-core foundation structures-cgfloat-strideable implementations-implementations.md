

- Core Foundation
- Core Foundation Structures
- CGFloat
-  Strideable Implementations 

API Collection

# Strideable Implementations

## Topics

### Instance Methods

func advanced(by: CGFloat) -> CGFloat

Returns a `Self` `x` such that `self.distance(to: x)` approximates `n`.

func distance(to: CGFloat) -> CGFloat

Returns a stride `x` such that `self.advanced(by: x)` approximates `other`.

