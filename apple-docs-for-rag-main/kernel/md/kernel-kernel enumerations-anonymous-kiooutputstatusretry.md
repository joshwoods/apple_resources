

- Kernel
- Kernel Enumerations
- Anonymous
-  kIOOutputStatusRetry 

Enumeration Case

# kIOOutputStatusRetry

macOS 10.12+

``` source
kIOOutputStatusRetry = 0x0002
```

## Discussion

Target ran out of resources, and is unable to accept the packet. The ownership of the packet reverts back to the queue.

