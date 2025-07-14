

- Foundation
- NSScriptClassDescription
-  isLocationRequiredToCreate(forKey:) 

Instance Method

# isLocationRequiredToCreate(forKey:)

Returns a Boolean value indicating whether an insertion location must be specified when creating a new object in the specified to-many relationship of the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
func isLocationRequiredToCreate(forKey toManyRelationshipKey: String) -> Bool
```

## Parameters 

`toManyRelationshipKey`  

The key for the to-many relationship that may require an insertion location.

## Return Value

true if an insertion location must be specified; otherwise, false.

## Discussion

A script command object that creates a new object in a to-many relationship needs to know whether an explicitly specified insertion location is required. It can get this information from an instance of `NSScriptClassDescription`. For example, `NSMakeCommand` uses this method to determine whether or not a specific `make` AppleScript command must have an `at` parameter.

## See Also

### Getting basic information about the script class

var className: String?

Returns the name of the class the receiver describes, as provided at initialization time.

var defaultSubcontainerAttributeKey: String?

Returns the value of the `DefaultSubcontainerAttribute` entry of the class dictionary from which the receiver was instantiated.

var implementationClassName: String?

Returns the name of the Objective-C class instantiated to implement the scripting class.

var suiteName: String?

Returns the name of the receiver’s suite.

