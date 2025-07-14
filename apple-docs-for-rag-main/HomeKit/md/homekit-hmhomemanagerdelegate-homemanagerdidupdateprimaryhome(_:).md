

- HomeKit
- HMHomeManagerDelegate
-  homeManagerDidUpdatePrimaryHome(\_:) 

Instance Method

# homeManagerDidUpdatePrimaryHome(\_:)

Tells the delegate that the home manager updated its primary home.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
optional func homeManagerDidUpdatePrimaryHome(_ manager: HMHomeManager)
```

## Parameters 

`manager`  

The home manager with an updated primary home.

## See Also

### Adding and removing homes

func homeManagerDidUpdateHomes(HMHomeManager)

Tells the delegate that the home manager updated its collection of homes.

func homeManager(HMHomeManager, didAdd: HMHome)

Tells the delegate that the home manager added a home.

func homeManager(HMHomeManager, didRemove: HMHome)

Tells the delegate that the home manager removed a home.

