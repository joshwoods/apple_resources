

- CarPlay
- CPMapTemplate
-  startNavigationSession(for:) 

Instance Method

# startNavigationSession(for:)

Begins navigational guidance for a trip.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
func startNavigationSession(for trip: CPTrip) -> CPNavigationSession
```

## Parameters 

`trip`  

The trip to provide guidance for.

## Return Value

A navigation session for the specified trip.

## Discussion

Keep a reference to the navigation session to perform guidance updates.

## See Also

### Navigating a Trip

class CPNavigationSession

An object that represents an active route guidance session.

