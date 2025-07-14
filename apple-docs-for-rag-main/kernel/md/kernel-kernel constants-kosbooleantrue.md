

- Kernel
- Kernel Constants
-  kOSBooleanTrue 

Global Variable

# kOSBooleanTrue

The OSBoolean constant for `true`.

macOS 10.0+

``` source
OSBoolean *const & kOSBooleanTrue;
```

## Discussion

kOSBooleanTrue is the OSBoolean constant for `true`. This object does not need to be retained or released (but it can be). Comparisons of the form `booleanObject == kOSBooleanTrue` are acceptable and are equivalent to `booleanObject->getValue() == true`.

