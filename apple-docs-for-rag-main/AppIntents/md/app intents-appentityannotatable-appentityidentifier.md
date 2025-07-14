

- App Intents
- AppEntityAnnotatable
-  appEntityIdentifier 

Instance Property

# appEntityIdentifier

The identifier of an app entity you set on framework types to make app content available to system experiences.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
var appEntityIdentifier: EntityIdentifier? { get set }
```

**Required**

## Discussion

Set this property to `nil` to clear the association between your AppEntity and the system type that adopts AppEntityAnnotatable.

