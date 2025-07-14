

- HomeKit
- HMError
-  objectAssociatedToAnotherHome 

Type Property

# objectAssociatedToAnotherHome

An attempt to associate an object with a home when it’s already associated with another home.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
static var objectAssociatedToAnotherHome: HMError.Code { get }
```

## See Also

### Detecting association errors

static var invalidAssociatedServiceType: HMError.Code

An error indicating an invalid service type.

static var objectAlreadyAssociatedToHome: HMError.Code

An attempt to associate an object with a home when it’s already associated with that home.

static var objectNotAssociatedToAnyHome: HMError.Code

An attempt to perform an operation on an object that is not associated to any home.

