

- Address Book
- ABGroup
-  addMember(\_:) 

Instance Method

# addMember(\_:)

Adds a person to a group.

macOS

``` source
func addMember(_ person: ABPerson!) -> Bool
```

## Parameters 

`person`  

The person record to be added.

## Return Value

true if successful; otherwise, false.

## Discussion

If the `person` argument is already part of the group, this method does nothing and returns true. If the `person` argument is `nil`, this method raises an exception.

### Special Considerations

Prior to OS X v10.6, if the person record is already in the group, this method does nothing and returns false.

## See Also

### Managing persons

func removeMember(ABPerson!) -> Bool

Removes a person from a group.

func members() -> [Any]!

Returns an array of persons in a group.

