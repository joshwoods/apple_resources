

- HomeKit
- HMHomeManager
-  removeHome(\_:completionHandler:) 

Instance Method

# removeHome(\_:completionHandler:)

Removes a home from this home manager.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+visionOS 1.0+

``` source
func removeHome(
    _ home: HMHome,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func removeHome(_ home: HMHome) async throws
```

## Parameters 

`home`  

The home to remove.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## Discussion

This method returns an error if the specified home is not managed by the home manager.

## See Also

### Adding and removing homes

func addHome(withName: String, completionHandler: (HMHome?, (any Error)?) -> Void)

Adds a new home to this home manager.

