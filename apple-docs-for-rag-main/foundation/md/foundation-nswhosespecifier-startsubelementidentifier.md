

- Foundation
- NSWhoseSpecifier
-  startSubelementIdentifier 

Instance Property

# startSubelementIdentifier

Returns the start sub-element identifier for the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
var startSubelementIdentifier: NSWhoseSpecifier.SubelementIdentifier { get set }
```

## Return Value

The start sub-element identifier for the receiver.

## See Also

### Accessing information about a whose specifier

var endSubelementIdentifier: NSWhoseSpecifier.SubelementIdentifier

Sets the end sub-element identifier for the specifier to the value of a given sub-element.

var endSubelementIndex: Int

Sets the index position of the last sub-element within the range of objects being tested that pass the specifier’s test.

var startSubelementIndex: Int

Returns the index position of the first sub-element within the range of objects being tested that pass the receiver’s test.

var test: NSScriptWhoseTest

Returns the test object encapsulated by the receiver.

