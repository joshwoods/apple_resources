

- Local Authentication
- LAEnvironment
- LAEnvironment.MechanismCompanion
-  stateHash 

Instance Property

# stateHash

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
var stateHash: Data? { get }
```

## Discussion

```
        If at least one companion is paired for this companion type, @c stateHash is not @c nil and
        it changes whenever the set of paired companions of this type is changed.
```

