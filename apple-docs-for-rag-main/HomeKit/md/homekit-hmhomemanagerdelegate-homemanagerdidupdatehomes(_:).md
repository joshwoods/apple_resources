

- HomeKit
- HMHomeManagerDelegate
-  homeManagerDidUpdateHomes(\_:) 

Instance Method

# homeManagerDidUpdateHomes(\_:)

Tells the delegate that the home manager updated its collection of homes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
optional func homeManagerDidUpdateHomes(_ manager: HMHomeManager)
```

## Parameters 

`manager`  

The home manager with updated homes.

## Discussion

The home manager calls this method to inform an application of significant changes to the home configuration, including when the manager finishes its first load of data from the HomeKit database on initialization. Use this method as a cue to invalidate any references to HomeKit objects and refresh your app’s views with the new list of homes.

## See Also

### Adding and removing homes

func homeManager(HMHomeManager, didAdd: HMHome)

Tells the delegate that the home manager added a home.

func homeManager(HMHomeManager, didRemove: HMHome)

Tells the delegate that the home manager removed a home.

func homeManagerDidUpdatePrimaryHome(HMHomeManager)

Tells the delegate that the home manager updated its primary home.

