

- Quartz
- QCPlugIn
-  plugInKeys() Deprecated

Type Method

# plugInKeys()

Returns the keys for the internal settings of a custom patch.

macOS 10.4–10.15Deprecated

``` source
class func plugInKeys() -> [Any]!
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

An array of keys used for key-value coding (KVC) of the internal settings.

## Discussion

You must override this method if your patch provides a Settings pane. This keys are used for automatic serialization of the internal settings and are also used by the QCPlugInViewController instance for the Settings pane. The implementation is straightforward; the keys are strings that represent the instance variables used for the Settings pane. For example, the `plugInKeys` method for these instance variables:

```
@property(ivar, byref) NSColor * systemColor;
@property(ivar, byref) NSConfiguration * systemConfiguration;
```

are:

```
+ (NSArray*) plugInKeys
{
    return [NSArray arrayWithObjects: @"systemColor",
                                      @"systemConfiguration",
                                      nil];
}
```

## See Also

### Defining Internal Settings

func createViewController() -> QCPlugInViewController!

Creates and returns a view controller for the Settings pane of a custom patch.

Deprecated

