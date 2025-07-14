

- Kernel
- IOKit Fundamentals
- IOService
-  setNotification 

Type Method

# setNotification

macOS 10.11.4+

``` source
static OSPtr setNotification(const OSSymbol *type, OSDictionary *matching, IOServiceMatchingNotificationHandler handler, void *target, void *ref, SInt32 priority);
```

