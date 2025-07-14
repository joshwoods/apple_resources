

- Group Activities
- GroupStateObserver
-  isEligibleForGroupSession 

Instance Property

# isEligibleForGroupSession

A Boolean value that indicates whether the system can start a group session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
@Published
final var isEligibleForGroupSession: Bool { get }
```

## Mentioned in 

Presenting SharePlay activities from your app’s UI

## Discussion

This property indicates whether a FaceTime call is active and the system can create group sessions. Configure a subscriber to this property to monitor changes to the system’s state. When the system can create group sessions, it sets the value of this property to `true`. When the creation of a group session isn’t possible, the system sets the value to `false`.

