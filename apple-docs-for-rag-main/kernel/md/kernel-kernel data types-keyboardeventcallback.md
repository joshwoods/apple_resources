

- Kernel
- Kernel Data Types
-  KeyboardEventCallback 

Type Alias

# KeyboardEventCallback

macOS 10.3+

``` source
typedef void (*KeyboardEventCallback)(OSObject *target, unsigned int eventType, unsigned int flags, unsigned int key, unsigned int charCode, unsigned int charSet, unsigned int origCharCode, unsigned int origCharSet, unsigned int keyboardType, bool repeat, AbsoluteTime ts, OSObject *sender, void *refcon);
```

