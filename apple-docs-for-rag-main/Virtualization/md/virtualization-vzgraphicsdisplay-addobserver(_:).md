

- Virtualization
- VZGraphicsDisplay
-  addObserver(\_:) 

Instance Method

# addObserver(\_:)

Adds an observer to notify about display configuration changes.

macOS 14.0+

``` source
func addObserver(_ observer: any VZGraphicsDisplayObserver)
```

## Parameters 

`observer`  

The new observer the framework notifies about display configuration changes.

## See Also

### Observing changes to the display configuration

func removeObserver(any VZGraphicsDisplayObserver)

Removes a display configuration change observer.

protocol VZGraphicsDisplayObserver

A protocol you implement to observe state changes in graphic displays.

