

- Kernel
- Kernel Enumerations
- Anonymous
-  kIONetworkFeatureNoBSDWait 

Enumeration Case

# kIONetworkFeatureNoBSDWait

macOS 10.12+

``` source
kIONetworkFeatureNoBSDWait = 0x001
```

## Discussion

Set this bit in the value returned by getFeatures() to disable the automatic wait for "IOBSD" resource by the IONetworkController::start() method.

