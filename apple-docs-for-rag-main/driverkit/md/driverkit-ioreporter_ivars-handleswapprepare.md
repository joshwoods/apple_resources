

- DriverKit
- IOReporter_IVars
-  handleSwapPrepare 

Instance Method

# handleSwapPrepare

DriverKitiOSiPadOSmacOS

``` source
IOReturn handleSwapPrepare(int newNChannels);
```

## Parameters 

`newNChannels`  

Target number of channels

## Return Value

IOReturn code

## Discussion

::handleSwapPrepare() is responsible for allocating appropriately- sized buffers (based on the new number of channels) and storing them in \_swap\* instance variables. If returning and error, it must deallocate any buffers and set to NULL any \_swap\* variables.

Locking: The caller must ensure that the *config* lock is HELD but that the reporter (data) lock is *NOT HELD*.

