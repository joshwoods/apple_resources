

- HomeKit
- HMActionSet
-  name 

Instance Property

# name

The name of the action set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var name: String { get }
```

## Discussion

Action set names must be unique within a home.

## See Also

### Related Documentation

HomeKit Developer Guide

### Identifiying an action set

var uniqueIdentifier: UUID

The action set’s unique identifier.

func updateName(String, completionHandler: HMErrorBlock)

Updates the name of the action set.

