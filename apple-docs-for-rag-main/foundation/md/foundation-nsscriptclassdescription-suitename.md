

- Foundation
- NSScriptClassDescription
-  suiteName 

Instance Property

# suiteName

Returns the name of the receiver’s suite.

Mac Catalyst 13.0+macOS 10.0+

``` source
var suiteName: String? { get }
```

## Return Value

The receiver’s suite name. Within an application’s scriptability information, named suites contain related sets of information.

## See Also

### Getting basic information about the script class

var className: String?

Returns the name of the class the receiver describes, as provided at initialization time.

var defaultSubcontainerAttributeKey: String?

Returns the value of the `DefaultSubcontainerAttribute` entry of the class dictionary from which the receiver was instantiated.

var implementationClassName: String?

Returns the name of the Objective-C class instantiated to implement the scripting class.

func isLocationRequiredToCreate(forKey: String) -> Bool

Returns a Boolean value indicating whether an insertion location must be specified when creating a new object in the specified to-many relationship of the receiver.

