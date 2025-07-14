

- Group Activities
- SystemCoordinator
-  localParticipantStates 

Instance Property

# localParticipantStates

An asynchronous sequence that reports changes to the local participant’s state.

visionOS 1.0+

``` source
final var localParticipantStates: SystemCoordinator.ParticipantStates { get }
```

## Mentioned in 

Adding spatial Persona support to an activity

## Discussion

Use this property to detect when the current person starts or stops displaying their spatial Persona. The following example shows how to set up a task to monitor the sequence and respond to changes:

```
Task.detached {
    for await localParticipantState in systemCoordinator.localParticipantStates {
         if localParticipantState.isSpatial {
              // Handle changes to the state.
         }
    }
}
```

## See Also

### Getting the participant state

var localParticipantState: SystemCoordinator.ParticipantState

The current participant’s level of support for an activity that takes place in a shared simulation space.

struct ParticipantStates

An asynchronous sequence that reports the current person’s ability to participate in a shared context.

