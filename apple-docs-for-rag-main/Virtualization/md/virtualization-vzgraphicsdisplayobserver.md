

- Virtualization
-  VZGraphicsDisplayObserver 

Protocol

# VZGraphicsDisplayObserver

A protocol you implement to observe state changes in graphic displays.

macOS 14.0+

``` source
protocol VZGraphicsDisplayObserver : NSObjectProtocol
```

## Overview

Implement the methods in this protocol to observe and react to display reconfiguration.

## Topics

### Reacting to changes in display configuration

func displayDidBeginReconfiguration(VZGraphicsDisplay)

The method the framework calls when the reconfiguration operation has begun.

func displayDidEndReconfiguration(VZGraphicsDisplay)

The method the framework calls when the reconfiguration operation ends.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Observing changes to the display configuration

func addObserver(any VZGraphicsDisplayObserver)

Adds an observer to notify about display configuration changes.

func removeObserver(any VZGraphicsDisplayObserver)

Removes a display configuration change observer.

