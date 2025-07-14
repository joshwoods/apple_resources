

- Foundation
- NSScriptClassDescription
-  className 

Instance Property

# className

Returns the name of the class the receiver describes, as provided at initialization time.

Mac Catalyst 13.0+macOS 10.0+

``` source
var className: String? { get }
```

## Return Value

A class name. This may be either the human-readable name for the class—that is, the name that is used in a script—or the name of the Objective-C class that is instantiated to implement the class. To reliably obtain the implementation name, use implementationClassName.

## See Also

### Getting basic information about the script class

var defaultSubcontainerAttributeKey: String?

Returns the value of the `DefaultSubcontainerAttribute` entry of the class dictionary from which the receiver was instantiated.

var implementationClassName: String?

Returns the name of the Objective-C class instantiated to implement the scripting class.

func isLocationRequiredToCreate(forKey: String) -> Bool

Returns a Boolean value indicating whether an insertion location must be specified when creating a new object in the specified to-many relationship of the receiver.

var suiteName: String?

Returns the name of the receiver’s suite.

