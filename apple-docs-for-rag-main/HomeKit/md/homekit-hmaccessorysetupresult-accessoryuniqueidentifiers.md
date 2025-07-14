

- HomeKit
- HMAccessorySetupResult
-  accessoryUniqueIdentifiers 

Instance Property

# accessoryUniqueIdentifiers

The values corresponding to accessories that are set up.

iOS 15.4+iPadOS 15.4+

``` source
var accessoryUniqueIdentifiers: [UUID] { get }
```

## Discussion

Usually only one accessory is set up at a time, but adding an accessory bridge can result in multiple accessories being set up at once. See uniqueIdentifier for more information.

## See Also

### Getting results

var homeUniqueIdentifier: UUID

The home that accessories were added to.

