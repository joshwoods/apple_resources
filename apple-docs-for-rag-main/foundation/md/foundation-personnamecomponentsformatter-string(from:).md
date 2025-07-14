

- Foundation
- PersonNameComponentsFormatter
-  string(from:) 

Instance Method

# string(from:)

Returns a string formatted for a given `NSPersonNameComponents` object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func string(from components: PersonNameComponents) -> String
```

## Parameters 

`components`  

The name components to be formatted.

## Return Value

A formatted string representation of the given name components.

## See Also

### Converting Between Person Name Components and Strings

class func localizedString(from: PersonNameComponents, style: PersonNameComponentsFormatter.Style, options: PersonNameComponentsFormatter.Options) -> String

Returns a string formatted for a given `NSPersonNameComponents` object using the provided style and options.

func annotatedString(from: PersonNameComponents) -> NSAttributedString

Returns an attributed string formatted for a given `NSPersonNameComponents` object, with attribute annotations for each component.

func personNameComponents(from: String) -> PersonNameComponents?

Returns a person name components object from a given string.

func getObjectValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>?, for: String, errorDescription: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

Returns by reference a person name components object after creating it from a given string.

