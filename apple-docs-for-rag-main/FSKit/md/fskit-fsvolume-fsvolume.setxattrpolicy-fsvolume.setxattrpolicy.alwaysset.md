

- FSKit
- FSVolume
- FSVolume.SetXattrPolicy
-  FSVolume.SetXattrPolicy.alwaysSet 

Case

# FSVolume.SetXattrPolicy.alwaysSet

Set the value, regardless of previous state.

macOS 15.4+

``` source
case alwaysSet
```

## See Also

### Declaring a policy

case mustCreate

Set the value, but fail if the extended attribute already exists.

case mustReplace

Set the value, but fail if the extended attribute doesn’t already exist.

case delete

Delete the value, failing if the extended attribute doesn’t exist.

