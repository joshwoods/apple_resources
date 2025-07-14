

- Core Graphics
- CGDataConsumerCallbacks
-  putBytes 

Instance Property

# putBytes

A pointer to a function that copies data to the data consumer. For more information, see CGDataConsumerPutBytesCallback.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var putBytes: CGDataConsumerPutBytesCallback?
```

## See Also

### Instance Properties

var releaseConsumer: CGDataConsumerReleaseInfoCallback?

A pointer to a function that handles clean-up for the data consumer, or `NULL`.

