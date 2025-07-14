

- DriverKit
- IOReporter_IVars
-  handleSwapCleanup 

Instance Method

# handleSwapCleanup

DriverKitiOSiPadOSmacOS

``` source
void handleSwapCleanup(int swapNChannels);
```

## Parameters 

`swapNChannels`  

Channel-Relative size of the \_swap buffers

## Discussion

::handleSwapCleanup() is responsible for deallocating the buffers no longer used after a swap. It must always be called if SwapPrepare() completes successfully. Because bufers may be swapped in and out of existance, the \_swap\* variables may be NULL and should be set to NULL when complete.

Locking: The caller must ensure that the *config* lock is HELD but that the reporter (data) lock is *NOT HELD*.

