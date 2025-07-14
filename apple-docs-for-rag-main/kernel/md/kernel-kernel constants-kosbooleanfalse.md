

- Kernel
- Kernel Constants
-  kOSBooleanFalse 

Global Variable

# kOSBooleanFalse

The OSBoolean constant for `false`.

macOS 10.0+

``` source
OSBoolean *const & kOSBooleanFalse;
```

## Discussion

kOSBooleanFalse is the OSBoolean constant for `false`. This object does not need to be retained or released (but it can be). Comparisons of the form `booleanObject == kOSBooleanFalse` are acceptable and are equivalent to `booleanObject->getValue() == false`.

