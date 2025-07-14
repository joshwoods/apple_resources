

- Group Activities
- SpatialTemplateConfiguration
-  init(defaultInitiatorRole:) 

Initializer

# init(defaultInitiatorRole:)

Creates the configuration structure for a spatial template.

visionOS 2.0+

``` source
init(defaultInitiatorRole: (any SpatialTemplateRole)? = nil)
```

## Parameters 

`defaultInitiatorRole`  

The template-specific role to apply to the person who initiates the activity. The specified role must be present in the template. Specify `nil` if you don’t want to assign a specific role to the initiator of the activity.

## Return Value

An initialized configuration object.

