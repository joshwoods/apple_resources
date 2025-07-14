

- Audio Toolbox
- AudioFileStreamPropertyFlags
-  propertyIsCached 

Type Property

# propertyIsCached

This flag is set when the callback AudioFileStream_PropertyListenerProc is invoked in the case that the value of the property has been cached and can be obtained later.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
static var propertyIsCached: AudioFileStreamPropertyFlags { get }
```

## Discussion

If this flag is not set, get the value of the property from within this callback or set the cacheProperty flag to instruct the parser to begin caching the property data. Otherwise, the value will not be available after the callback returns.

## See Also

### Constants

static var cacheProperty: AudioFileStreamPropertyFlags

A property listener sets this flag to instruct the parser to cache the property value so that it remains available after the callback returns.

