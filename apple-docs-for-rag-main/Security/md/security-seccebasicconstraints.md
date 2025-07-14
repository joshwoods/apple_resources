

- Security
-  SecCEBasicConstraints 

Structure

# SecCEBasicConstraints

Mac Catalyst 13.0+

``` source
struct SecCEBasicConstraints
```

## Topics

### Initializers

init()

init(present: Bool, critical: Bool, isCA: Bool, pathLenConstraintPresent: Bool, pathLenConstraint: UInt32)

### Instance Properties

var critical: Bool

var isCA: Bool

var pathLenConstraint: UInt32

var pathLenConstraintPresent: Bool

var present: Bool

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

