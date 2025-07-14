

- HomeKit
- HMError
-  invalidAssociatedServiceType 

Type Property

# invalidAssociatedServiceType

An error indicating an invalid service type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
static var invalidAssociatedServiceType: HMError.Code { get }
```

## See Also

### Detecting association errors

static var objectAlreadyAssociatedToHome: HMError.Code

An attempt to associate an object with a home when it’s already associated with that home.

static var objectAssociatedToAnotherHome: HMError.Code

An attempt to associate an object with a home when it’s already associated with another home.

static var objectNotAssociatedToAnyHome: HMError.Code

An attempt to perform an operation on an object that is not associated to any home.

