

- Kernel
- Kernel Data Types
-  BPF_FUNC 

Type Alias

# BPF_FUNC

macOS 10.6+

``` source
typedef int (*BPF_FUNC)(struct ifnet *, struct mbuf *);
```

## Discussion

Prototype for the BPF tap handler. This will disappear when the correct DLIL header file is included.

