

- Kernel
- IOKit Fundamentals
- Data Types
-  OSObjectApplierFunction 

Type Alias

# OSObjectApplierFunction

macOS 10.0+

``` source
typedef void (*OSObjectApplierFunction)(OSObject *object, void *context);
```

## See Also

### Callback Methods

OSActionAbortedHandler

OSActionCancelHandler

OSDispatchMethod

OSKextRequestResourceCallback

Invoked to provide results for a kext resource request.

OSSerializerBlock

OSSerializerCallback

