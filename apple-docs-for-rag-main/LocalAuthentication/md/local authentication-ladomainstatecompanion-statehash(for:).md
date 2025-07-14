

- Local Authentication
- LADomainStateCompanion
-  stateHash(for:) 

Instance Method

# stateHash(for:)

Returns state hash data for the given companion type.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
func stateHash(for companionType: LACompanionType) -> Data?
```

## Parameters 

`companionType`  

The companion type for which state hash data should be returned.

## Discussion

If database of paired devices of the given type was modified state hash data will change. Nature of such database changes cannot be determined but comparing data of state hash after different policy evaluation will reveal the fact database was changed between calls.

