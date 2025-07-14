

- DriverKit
- IOTimerDispatchSource
-  init 

Instance Method

# init

Handles the basic initialization of the dispatch source.

DriverKitiOSiPadOSmacOS

``` source
bool init();
```

## Return Value

true if initialization was successful, or false if an error occurred.

## Discussion

Don’t call this method directly. Call Create when you want to create a new timer dispatch queue.

## See Also

### Configuring the Timer Source

Create

Creates and configures a timer dispatch object.

free

Performs any final cleanup for the timer dispatch source.

SetHandler

Sets the handler block to run when the timer fires.

