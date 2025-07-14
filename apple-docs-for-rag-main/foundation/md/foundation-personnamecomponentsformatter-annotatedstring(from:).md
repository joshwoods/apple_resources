

- Foundation
- PersonNameComponentsFormatter
-  annotatedString(from:) 

Instance Method

# annotatedString(from:)

Returns an attributed string formatted for a given `NSPersonNameComponents` object, with attribute annotations for each component.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func annotatedString(from components: PersonNameComponents) -> NSAttributedString
```

## Parameters 

`components`  

A formatted string representation of the given name components.

## Return Value

An attributed string representation of the given name components. You can determine the person component corresponding to a particular range of the attributed string by querying the `NSPersonNameComponentKey` attribute, providing one of the `NSPersonNameComponent` constant values defined below as the attribute value.

## Discussion

Use this method to style individual components of a formatted name, such as a name in a label.

## See Also

### Converting Between Person Name Components and Strings

class func localizedString(from: PersonNameComponents, style: PersonNameComponentsFormatter.Style, options: PersonNameComponentsFormatter.Options) -> String

Returns a string formatted for a given `NSPersonNameComponents` object using the provided style and options.

func string(from: PersonNameComponents) -> String

Returns a string formatted for a given `NSPersonNameComponents` object.

func personNameComponents(from: String) -> PersonNameComponents?

Returns a person name components object from a given string.

func getObjectValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>?, for: String, errorDescription: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

Returns by reference a person name components object after creating it from a given string.

