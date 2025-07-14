

- Audio Toolbox
- AudioFileStreamPropertyFlags
-  cacheProperty 

Type Property

# cacheProperty

A property listener sets this flag to instruct the parser to cache the property value so that it remains available after the callback returns.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
static var cacheProperty: AudioFileStreamPropertyFlags { get }
```

## See Also

### Constants

static var propertyIsCached: AudioFileStreamPropertyFlags

This flag is set when the callback AudioFileStream_PropertyListenerProc is invoked in the case that the value of the property has been cached and can be obtained later.

