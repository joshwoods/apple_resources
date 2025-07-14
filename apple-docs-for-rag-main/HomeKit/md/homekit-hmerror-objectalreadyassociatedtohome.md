

- HomeKit
- HMError
-  objectAlreadyAssociatedToHome 

Type Property

# objectAlreadyAssociatedToHome

An attempt to associate an object with a home when it’s already associated with that home.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
static var objectAlreadyAssociatedToHome: HMError.Code { get }
```

## See Also

### Detecting association errors

static var invalidAssociatedServiceType: HMError.Code

An error indicating an invalid service type.

static var objectAssociatedToAnotherHome: HMError.Code

An attempt to associate an object with a home when it’s already associated with another home.

static var objectNotAssociatedToAnyHome: HMError.Code

An attempt to perform an operation on an object that is not associated to any home.

