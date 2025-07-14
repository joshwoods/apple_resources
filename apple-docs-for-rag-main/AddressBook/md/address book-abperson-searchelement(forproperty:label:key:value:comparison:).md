

- Address Book
- ABPerson
-  searchElement(forProperty:label:key:value:comparison:) 

Type Method

# searchElement(forProperty:label:key:value:comparison:)

Returns a search element object that specifies a query for records of this type.

macOS

``` source
class func searchElement(
    forProperty property: String!,
    label: String!,
    key: String!,
    value: Any!,
    comparison: ABSearchComparison
) -> ABSearchElement!
```

## Parameters 

`property`  

The name of the property to search on, such as `kABAddressProperty` or `kABLastNameProperty`. This name cannot be `nil`. For a full list of the properties, see Default Record Properties and Default Person Properties.

`label`  

The label name for a multivalue list, such as `kABAddressHomeLabel`, `kABPhoneWorkLabel`, or a user-specified label, such as `Summer Home`. If the specified property does not have multiple values, pass `nil`. If the specified property does have multiple values, pass `nil` to search all the values. For a full list of label names, see Default Multivalue List Labels and Generic Multivalue List Labels.

`key`  

The key name for a dictionary, such as `kABAddressCityKey` or `kABAddressStreetKey`. If the specified property is not a dictionary, pass `nil`. If the specified property is a dictionary, pass `nil` to search all keys. For a full list of key names, see Address Keys.

`value`  

What you’re searching for. If `nil`, then the only supported value for `comparison` is `kABEqual` or `kABNotEqual`.

`comparison`  

The type of comparison to perform, such as `kABEqual` or `kABPrefixMatchCaseInsensitive`.

