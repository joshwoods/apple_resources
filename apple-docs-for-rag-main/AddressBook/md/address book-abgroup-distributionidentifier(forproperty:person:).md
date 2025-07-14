

- Address Book
- ABGroup
-  distributionIdentifier(forProperty:person:) 

Instance Method

# distributionIdentifier(forProperty:person:)

Returns the distribution identifier for the given property and person.

macOS

``` source
func distributionIdentifier(
    forProperty property: String!,
    person: ABPerson!
) -> String!
```

## Parameters 

`property`  

The property whose distribution identifier will be returned.

`person`  

The person whose distribution identifier will be returned.

## Return Value

The distribution identifier for the given property and person.

## Discussion

If a distribution identifier is not set, this method returns the multivalue’s primary identifier. If either the `property` or the `person` argument is `nil`, this method returns `nil`. This method also returns `nil` if `property` is not a multivalue list property, or if `person` is not a member of the group.

Distribution identifiers let you use groups as distribution lists, by indicating which value in a multivalue property should be used when addressing the group. See Using Address Book Groups as Distribution Lists for more detailed discussion.

## See Also

### Managing Distribution Lists

func setDistributionIdentifier(String!, forProperty: String!, person: ABPerson!) -> Bool

Assigns a specific distribution identifier for a person’s multivalue list property so that the group can be used as a distribution list.

