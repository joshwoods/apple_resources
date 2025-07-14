

- FSKit
- FSVolume
- FSVolume.SetXattrPolicy
-  FSVolume.SetXattrPolicy.mustCreate 

Case

# FSVolume.SetXattrPolicy.mustCreate

Set the value, but fail if the extended attribute already exists.

macOS 15.4+

``` source
case mustCreate
```

## See Also

### Declaring a policy

case alwaysSet

Set the value, regardless of previous state.

case mustReplace

Set the value, but fail if the extended attribute doesn’t already exist.

case delete

Delete the value, failing if the extended attribute doesn’t exist.

