

- Local Authentication
- LAEnvironment
- LAEnvironment.MechanismBiometry
-  stateHash 

Instance Property

# stateHash

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
var stateHash: Data { get }
```

## Discussion

```
        It does not directly map to the enrolled templates, e.g. if a finger is added to Touch ID enrollement and then
        removed, the final state would be different.
        It also returns different values to different apps to prevent tracking of user identity.
```

