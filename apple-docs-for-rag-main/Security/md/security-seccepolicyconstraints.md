

- Security
-  SecCEPolicyConstraints 

Structure

# SecCEPolicyConstraints

Mac Catalyst 13.0+

``` source
struct SecCEPolicyConstraints
```

## Topics

### Initializers

init()

init(present: Bool, critical: Bool, requireExplicitPolicyPresent: Bool, requireExplicitPolicy: UInt32, inhibitPolicyMappingPresent: Bool, inhibitPolicyMapping: UInt32)

### Instance Properties

var critical: Bool

var inhibitPolicyMapping: UInt32

var inhibitPolicyMappingPresent: Bool

var present: Bool

var requireExplicitPolicy: UInt32

var requireExplicitPolicyPresent: Bool

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

