

- Group Activities
- SystemCoordinator
-  assignRole(\_:) 

Instance Method

# assignRole(\_:)

Assigns the given spatial template role to the local participant.

visionOS 2.0+

``` source
final func assignRole(_ role: some SpatialTemplateRole)
```

## Discussion

For example, in a table tennis game with two teams you might have the following:

```
switch selectedTeam {
case .blue:
    systemCoordinator.assignRole(TableTennisTemplate.Role.blueTeam)
case .red:
    systemCoordinator.assignRole(TableTennisTemplate.Role.redTeam)
}
```

Note that assigning a given role does not guarantee that the participant will be placed in a *seat* with that role. If more participants are assigned a role than there are seats for that role, the participant may be placed in a non-roled seat instead. In most cases, your app should try to avoid allowing for that scenario.

Warning

You should only assign roles that exist in the current spatial template.

This method will emit a runtime warning if the given role is not assigned to a seat in the current spatialTemplatePreference.

## See Also

### Assigning the local participant role

func resignRole()

Resigns the local participant from their current spatial template role.

