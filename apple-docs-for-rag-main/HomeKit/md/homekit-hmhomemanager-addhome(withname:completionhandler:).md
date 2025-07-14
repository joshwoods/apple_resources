

- HomeKit
- HMHomeManager
-  addHome(withName:completionHandler:) 

Instance Method

# addHome(withName:completionHandler:)

Adds a new home to this home manager.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+visionOS 1.0+

``` source
func addHome(
    withName homeName: String,
    completionHandler completion: @escaping (HMHome?, (any Error)?) -> Void
)
```

``` source
func addHome(named homeName: String) async throws -> HMHome
```

## Parameters 

`homeName`  

The name of the new home. Must not match the name of an existing home.

`completion`  

The block executed after the request is processed.

home  
The newly created home; may be `nil` if creation failed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Adding and removing homes

func removeHome(HMHome, completionHandler: ((any Error)?) -> Void)

Removes a home from this home manager.

