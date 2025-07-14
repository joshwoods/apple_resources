

- TipKit
- Tips
- Tips.ConfigurationOption
- Tips.ConfigurationOption.DatastoreLocation
-  groupContainer(identifier:) 

Type Method

# groupContainer(identifier:)

DatastoreLocation for persisting tips in a group container.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func groupContainer(identifier: String) throws -> Tips.ConfigurationOption.DatastoreLocation
```

## Parameters 

`identifier`  

A string that names the group whose shared directory you want to obtain. This input should exactly match one of the strings in the app’s App Groups Entitlement.

