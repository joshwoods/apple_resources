

- Contacts
- CNSaveRequest
-  removeSubgroup(\_:from:) 

Instance Method

# removeSubgroup(\_:from:)

Remove a subgroup from the specified parent group.

macOS 10.11+

``` source
func removeSubgroup(
    _ subgroup: CNGroup,
    from group: CNGroup
)
```

## Parameters 

`subgroup`  

The subgroup to remove.

`group`  

The parent group containing `subgroup`.

## Discussion

If you previously tried to add `subgroup` to `group` in the same save request, calling this method undoes that addition. The last change you make is the one that takes effect.

## See Also

### Adding and removing subgroups

func addSubgroup(CNGroup, to: CNGroup)

Add the specified group to a parent group.

