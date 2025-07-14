

- Address Book
- ABGroup
-  removeMember(\_:) 

Instance Method

# removeMember(\_:)

Removes a person from a group.

macOS

``` source
func removeMember(_ person: ABPerson!) -> Bool
```

## Parameters 

`person`  

The person to be removed.

## Return Value

true if successful; otherwise, false.

## Discussion

If the `person` argument is not in the group, this method does nothing and returns false. If `person` is `nil`, this method raises an exception.

## See Also

### Managing persons

func addMember(ABPerson!) -> Bool

Adds a person to a group.

func members() -> [Any]!

Returns an array of persons in a group.

