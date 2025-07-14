

- DriverKit
- IOCommandPool
-  returnCommand 

Instance Method

# returnCommand

DriverKitiOSiPadOSmacOS

``` source
void returnCommand(IOCommand * command);
```

## Parameters 

`command`  

The command to place in the pool.

## Discussion

The returnCommand method is used to place an object of type IOCommand into the pool, whether it be the first time, or the 1000th time.

