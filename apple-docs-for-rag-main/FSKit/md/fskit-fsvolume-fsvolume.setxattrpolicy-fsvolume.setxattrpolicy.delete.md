

- FSKit
- FSVolume
- FSVolume.SetXattrPolicy
-  FSVolume.SetXattrPolicy.delete 

Case

# FSVolume.SetXattrPolicy.delete

Delete the value, failing if the extended attribute doesn’t exist.

macOS 15.4+

``` source
case delete
```

## See Also

### Declaring a policy

case alwaysSet

Set the value, regardless of previous state.

case mustCreate

Set the value, but fail if the extended attribute already exists.

case mustReplace

Set the value, but fail if the extended attribute doesn’t already exist.

