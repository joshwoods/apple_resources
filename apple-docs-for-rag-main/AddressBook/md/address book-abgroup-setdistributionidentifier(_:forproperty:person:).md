

- Address Book
- ABGroup
-  setDistributionIdentifier(\_:forProperty:person:) 

Instance Method

# setDistributionIdentifier(\_:forProperty:person:)

Assigns a specific distribution identifier for a person’s multivalue list property so that the group can be used as a distribution list.

macOS

``` source
func setDistributionIdentifier(
    _ identifier: String!,
    forProperty property: String!,
    person: ABPerson!
) -> Bool
```

## Parameters 

`identifier`  

The identifier to be set as the distribution identifier

`property`  

The property whose distribution identifier will be set.

`person`  

The person whose distribution identifier will be.

## Return Value

true if successful; otherwise, false.

## Discussion

The default distribution identifier is a multivalue list’s primary identifier. If `person` is `nil`, this method raises an exception.

Distribution identifiers let you use groups as distribution lists, by indicating which value in a multivalue property should be used when addressing the group. See Address Book Programming Guide for Mac for more detailed discussion.

## See Also

### Managing Distribution Lists

func distributionIdentifier(forProperty: String!, person: ABPerson!) -> String!

Returns the distribution identifier for the given property and person.

