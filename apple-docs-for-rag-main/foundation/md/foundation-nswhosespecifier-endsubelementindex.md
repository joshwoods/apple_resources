

- Foundation
- NSWhoseSpecifier
-  endSubelementIndex 

Instance Property

# endSubelementIndex

Sets the index position of the last sub-element within the range of objects being tested that pass the specifier’s test.

Mac Catalyst 13.0+macOS 10.0+

``` source
var endSubelementIndex: Int { get set }
```

## Parameters 

`index`  

The index position of the end sub-element.

## Discussion

Used only if the end sub-element identifier is `NSIndexSubelement`.

## See Also

### Accessing information about a whose specifier

var endSubelementIdentifier: NSWhoseSpecifier.SubelementIdentifier

Sets the end sub-element identifier for the specifier to the value of a given sub-element.

var startSubelementIdentifier: NSWhoseSpecifier.SubelementIdentifier

Returns the start sub-element identifier for the receiver.

var startSubelementIndex: Int

Returns the index position of the first sub-element within the range of objects being tested that pass the receiver’s test.

var test: NSScriptWhoseTest

Returns the test object encapsulated by the receiver.

