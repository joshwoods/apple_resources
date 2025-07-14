

- Group Activities
- SystemCoordinator
-  groupImmersionStyle 

Instance Property

# groupImmersionStyle

The presentation style to apply to an immersive space for the current activity.

GroupActivitiesSwiftUIvisionOS 1.0+

``` source
final var groupImmersionStyle: SystemCoordinator.GroupImmersionStyles { get }
```

## Mentioned in 

Adding spatial Persona support to an activity

## Discussion

During an activity, the system uses this property to communicate the style for a currently open immersive space. When no participants are displaying an immersive space, the value of this property is `nil`. When any participant displays a space, the system sets the value for all participants to the immersion style of the newly presented space. When a participant presents a space with a different presentation style, the system also updates the property to reflect the new style. For example, if the group is currently in a space with the full style, it updates the property when someone presents a space with the full style.

Use this property to synchronize the level of immersion for all participants. Keeping the participants at the same level of immersion preserves the shared context of your activity. When the value of the property changes, transition the current participant to the new immersion level only if doing so doesn’t disrupt any other ongoing tasks. For example, if the current person is editing content in an unrelated window, don’t transition them automatically. Instead, give them the choice of when to make the transition.

## See Also

### Getting the current immersion level

struct GroupImmersionStyles

An asynchronous sequence that contains one or more incoming immersion styles for you to process.

