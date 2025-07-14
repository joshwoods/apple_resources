

- Foundation
- NSPersonNameComponents
-  phoneticRepresentation 

Instance Property

# phoneticRepresentation

The phonetic representation name components of the receiver.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var phoneticRepresentation: PersonNameComponents? { get set }
```

## Discussion

Each component of the receiver with a value should have a corresponding value for any value set for this property. `nil` by default.

The `phoneticRepresentation` property value of this property value is ignored.

## See Also

### Accessing Person Name Components

var namePrefix: String?

The portion of a name’s full form of address that precedes the name itself *(for example, “Dr.,” “Mr.,” “Ms.”)*.

var givenName: String?

Name bestowed upon an individual to differentiate them from other members of a group that share a family name *(for example, “Johnathan”)*.

var middleName: String?

Secondary name bestowed upon an individual to differentiate them from others that have the same given name *(for example, “Maple”)*.

var familyName: String?

Name bestowed upon an individual to denote membership in a group or family. *(for example, “Appleseed”)*.

var nameSuffix: String?

The portion of a name’s full form of address that follows the name itself *(for example, “Esq.,” “Jr.,” “Ph.D.”)*.

var nickname: String?

Name substituted for the purposes of familiarity *(for example, “Johnny”)*.

