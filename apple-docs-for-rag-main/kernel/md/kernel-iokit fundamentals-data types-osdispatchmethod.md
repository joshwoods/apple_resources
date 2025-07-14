

- Kernel
- IOKit Fundamentals
- Data Types
-  OSDispatchMethod 

Type Alias

# OSDispatchMethod

macOS 10.15+

``` source
typedef kern_return_t (*OSDispatchMethod)(OSMetaClassBase *self, const IORPC rpc);
```

## See Also

### Callback Methods

OSActionAbortedHandler

OSActionCancelHandler

OSKextRequestResourceCallback

Invoked to provide results for a kext resource request.

OSObjectApplierFunction

OSSerializerBlock

OSSerializerCallback

