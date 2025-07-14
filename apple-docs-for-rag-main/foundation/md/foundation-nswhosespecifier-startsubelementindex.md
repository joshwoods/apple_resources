

- Foundation
- NSWhoseSpecifier
-  startSubelementIndex 

Instance Property

# startSubelementIndex

Returns the index position of the first sub-element within the range of objects being tested that pass the receiver’s test.

Mac Catalyst 13.0+macOS 10.0+

``` source
var startSubelementIndex: Int { get set }
```

## Return Value

The index position of the first sub-element within the range of objects being tested that pass the receiver’s test.

## See Also

### Accessing information about a whose specifier

var endSubelementIdentifier: NSWhoseSpecifier.SubelementIdentifier

Sets the end sub-element identifier for the specifier to the value of a given sub-element.

var endSubelementIndex: Int

Sets the index position of the last sub-element within the range of objects being tested that pass the specifier’s test.

var startSubelementIdentifier: NSWhoseSpecifier.SubelementIdentifier

Returns the start sub-element identifier for the receiver.

var test: NSScriptWhoseTest

Returns the test object encapsulated by the receiver.

