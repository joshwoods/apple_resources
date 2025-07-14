

- Virtualization
- VZGraphicsDisplay
-  removeObserver(\_:) 

Instance Method

# removeObserver(\_:)

Removes a display configuration change observer.

macOS 14.0+

``` source
func removeObserver(_ observer: any VZGraphicsDisplayObserver)
```

## Parameters 

`observer`  

The observer to remove from notifications about display configuration changes.

## See Also

### Observing changes to the display configuration

func addObserver(any VZGraphicsDisplayObserver)

Adds an observer to notify about display configuration changes.

protocol VZGraphicsDisplayObserver

A protocol you implement to observe state changes in graphic displays.

