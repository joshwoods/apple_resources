

- App Intents
- SetFocusFilterIntent
-  appContext 

Instance Property

# appContext

An app context that is associated with the focus configuration. The system will retrieve this app context and adapt the system behavior based on the context provided.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var appContext: FocusFilterAppContext { get }
```

**Required** Default implementation provided.

## Default Implementations

### SetFocusFilterIntent Implementations

var appContext: FocusFilterAppContext

An app context that is associated with the focus configuration. The system will retrieve this app context and adapt the system behavior based on the context provided.

## See Also

### Configuring app context for the Focus

static func invalidateFocusFilterAppContext()

