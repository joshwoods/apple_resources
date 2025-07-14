

- Kernel
- Kernel Data Types
-  kauth_scope_callback_t 

Type Alias

# kauth_scope_callback_t

macOS 11.0+

``` source
typedef int (*kauth_scope_callback_t)(kauth_cred_t _credential, void *_idata, kauth_action_t _action, uintptr_t _arg0, uintptr_t _arg1, uintptr_t _arg2, uintptr_t _arg3);
```

