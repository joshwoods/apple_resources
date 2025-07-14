

- HomeKit
- HMLocationEvent
-  init(region:) 

Initializer

# init(region:)

Creates a new location event with the specified region.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+

``` source
init(region: CLRegion)
```

## Parameters 

`region`  

Region on which the event is triggered. The region object must have at least one of notifyOnEntry or notifyOnExit set to true.

## Return Value

An initialized instance representing the location event.

