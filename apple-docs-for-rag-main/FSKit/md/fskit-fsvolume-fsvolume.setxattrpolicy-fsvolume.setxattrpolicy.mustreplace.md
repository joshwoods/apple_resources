

- FSKit
- FSVolume
- FSVolume.SetXattrPolicy
-  FSVolume.SetXattrPolicy.mustReplace 

Case

# FSVolume.SetXattrPolicy.mustReplace

Set the value, but fail if the extended attribute doesn’t already exist.

macOS 15.4+

``` source
case mustReplace
```

## See Also

### Declaring a policy

case alwaysSet

Set the value, regardless of previous state.

case mustCreate

Set the value, but fail if the extended attribute already exists.

case delete

Delete the value, failing if the extended attribute doesn’t exist.

