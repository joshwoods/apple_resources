

- Quartz
- QCCompositionRenderer
-  userInfo() Deprecated

Instance Method

# userInfo()

Returns a mutable dictionary for storing arbitrary information.

macOS 10.4–10.15Deprecated

``` source
func userInfo() -> NSMutableDictionary!
```

**Required**

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

A mutable dictionary.

## Discussion

The `userInfo` dictionary is shared—there is one per Quartz Composer context. In fact, it is the same dictionary as the one available for the plug-in execution context for instances of the QCPlugIn class.

When you add information to the dictionary, make sure that you use unique keys, such as `“com.myCompany.foo”`.

