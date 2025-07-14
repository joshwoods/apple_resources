

- Kernel
- IOKit Fundamentals
- IOService
-  doInstallNotification 

Type Method

# doInstallNotification

macOS 10.11.4+

``` source
static OSPtr doInstallNotification(const OSSymbol *type, OSDictionary *matching, IOServiceMatchingNotificationHandler handler, void *target, void *ref, SInt32 priority, OSIterator **existing);
```

