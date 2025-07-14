

- HomeKit
- HMHomeManagerDelegate
-  homeManager(\_:didAdd:) 

Instance Method

# homeManager(\_:didAdd:)

Tells the delegate that the home manager added a home.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
optional func homeManager(
    _ manager: HMHomeManager,
    didAdd home: HMHome
)
```

## Parameters 

`manager`  

The home manager that added the home.

`home`  

The newly added home.

## See Also

### Adding and removing homes

func homeManagerDidUpdateHomes(HMHomeManager)

Tells the delegate that the home manager updated its collection of homes.

func homeManager(HMHomeManager, didRemove: HMHome)

Tells the delegate that the home manager removed a home.

func homeManagerDidUpdatePrimaryHome(HMHomeManager)

Tells the delegate that the home manager updated its primary home.

