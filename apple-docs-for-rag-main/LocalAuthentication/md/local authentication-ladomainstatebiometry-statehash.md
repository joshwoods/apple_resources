

- Local Authentication
- LADomainStateBiometry
-  stateHash 

Instance Property

# stateHash

Contains state hash data for the available biometry type. Returns `nil` if no biometry entities are enrolled.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var stateHash: Data? { get }
```

## Discussion

If biometric database was modified (fingers, faces were removed or added), `stateHash` data will change. Nature of such database changes cannot be determined but comparing data of `stateHash` after different evaluatePolicy calls will reveal the fact database was changed between the calls.

```
     the state of biometry has not changed.
```

