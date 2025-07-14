

- InputMethodKit
- IMKCandidates
-  init(server:panelType:) 

Initializer

# init(server:panelType:)

Returns the initialized `IMKCandidates` object.

macOS 10.5+

``` source
@MainActor
init!(
    server: IMKServer!,
    panelType: IMKCandidatePanelType
)
```

## Parameters 

`server`  

The `IMKServer` object that manages the candidate and the panel type.

`panelType`  

A panel type for the candidate window.

## Return Value

The initialized `IMKCandidates` object.

## Discussion

When an input method allocates an `IMKCandidates` object it should initialize that object by calling this method.

