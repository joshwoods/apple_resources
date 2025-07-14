

- Foundation
- NSWhoseSpecifier
-  test 

Instance Property

# test

Returns the test object encapsulated by the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
var test: NSScriptWhoseTest { get set }
```

## Return Value

The test object encapsulated by the receiver.

## See Also

### Accessing information about a whose specifier

var endSubelementIdentifier: NSWhoseSpecifier.SubelementIdentifier

Sets the end sub-element identifier for the specifier to the value of a given sub-element.

var endSubelementIndex: Int

Sets the index position of the last sub-element within the range of objects being tested that pass the specifier’s test.

var startSubelementIdentifier: NSWhoseSpecifier.SubelementIdentifier

Returns the start sub-element identifier for the receiver.

var startSubelementIndex: Int

Returns the index position of the first sub-element within the range of objects being tested that pass the receiver’s test.

