

- HomeKit
- HMHomeManagerDelegate
-  homeManager(\_:didRemove:) 

Instance Method

# homeManager(\_:didRemove:)

Tells the delegate that the home manager removed a home.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
optional func homeManager(
    _ manager: HMHomeManager,
    didRemove home: HMHome
)
```

## Parameters 

`manager`  

The home manager that removed the home.

`home`  

The removed home.

## See Also

### Adding and removing homes

func homeManagerDidUpdateHomes(HMHomeManager)

Tells the delegate that the home manager updated its collection of homes.

func homeManager(HMHomeManager, didAdd: HMHome)

Tells the delegate that the home manager added a home.

func homeManagerDidUpdatePrimaryHome(HMHomeManager)

Tells the delegate that the home manager updated its primary home.

