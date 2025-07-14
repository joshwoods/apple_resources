

- Kernel
- IOKit Fundamentals
- Data Types
-  OSSerializerCallback 

Type Alias

# OSSerializerCallback

macOS 10.0+

``` source
typedef bool (*OSSerializerCallback)(void *target, void *ref, OSSerialize *serializer);
```

## See Also

### Callback Methods

OSActionAbortedHandler

OSActionCancelHandler

OSDispatchMethod

OSKextRequestResourceCallback

Invoked to provide results for a kext resource request.

OSObjectApplierFunction

OSSerializerBlock

