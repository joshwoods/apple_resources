

- Foundation
- NSWhoseSpecifier
-  endSubelementIdentifier 

Instance Property

# endSubelementIdentifier

Sets the end sub-element identifier for the specifier to the value of a given sub-element.

Mac Catalyst 13.0+macOS 10.0+

``` source
var endSubelementIdentifier: NSWhoseSpecifier.SubelementIdentifier { get set }
```

## Parameters 

`subelement`  

The end sub-element for the receiver.

## See Also

### Accessing information about a whose specifier

var endSubelementIndex: Int

Sets the index position of the last sub-element within the range of objects being tested that pass the specifier’s test.

var startSubelementIdentifier: NSWhoseSpecifier.SubelementIdentifier

Returns the start sub-element identifier for the receiver.

var startSubelementIndex: Int

Returns the index position of the first sub-element within the range of objects being tested that pass the receiver’s test.

var test: NSScriptWhoseTest

Returns the test object encapsulated by the receiver.

