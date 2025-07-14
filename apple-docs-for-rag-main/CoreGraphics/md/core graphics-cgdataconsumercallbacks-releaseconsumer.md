

- Core Graphics
- CGDataConsumerCallbacks
-  releaseConsumer 

Instance Property

# releaseConsumer

A pointer to a function that handles clean-up for the data consumer, or `NULL`.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var releaseConsumer: CGDataConsumerReleaseInfoCallback?
```

## Discussion

For more information, see CGDataConsumerReleaseInfoCallback.

## See Also

### Instance Properties

var putBytes: CGDataConsumerPutBytesCallback?

A pointer to a function that copies data to the data consumer. For more information, see CGDataConsumerPutBytesCallback.

