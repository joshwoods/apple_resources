

- Local Authentication
- LADomainStateCompanion
-  stateHash 

Instance Property

# stateHash

Contains combined state hash data for all available companion types. . Returns `nil` if no companion devices are paired.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
var stateHash: Data? { get }
```

## Discussion

As long as database of paired companion devices doesn’t change, `stateHash` stays the same for the same set of `availableCompanions`.

```
         If database of paired companion devices was modified, `stateHash`
         data will change. Nature of such database changes cannot be determined
         but comparing data of `stateHash` after different policy evaluation
         will reveal the fact database was changed between calls.

         If you are interested in a state hash for a specific companion type
         you can use `stateHashForCompanionType` method.
```

```
     the list of paired companions has not changed.
```

