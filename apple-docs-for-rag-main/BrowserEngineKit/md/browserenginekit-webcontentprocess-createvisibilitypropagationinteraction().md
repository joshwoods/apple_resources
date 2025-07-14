

- BrowserEngineKit
- WebContentProcess
-  createVisibilityPropagationInteraction() 

Instance Method

# createVisibilityPropagationInteraction()

Returns an interaction that associates a view with the web content process.

iOS 17.4+iPadOS 17.4+macOS 14.3+

``` source
func createVisibilityPropagationInteraction() -> any UIInteraction
```

## Overview

When you add a visibility propagation interaction to a view, the operating system treats the extension process as “visible” whenever the view is visible, and schedules the process as if it has visible UI. When the view is not visible, the operating system schedules the process as a background helper.

If your web content extension prepares content for multiple views, create a separate visibility propagation for each view.

## See Also

### Visibility propagation

Propagating view visibility information to extension processes

Register the extensions that contribute to preparing your browser app’s UI.

func createVisibilityPropagationInteraction() -> any UIInteraction

Returns an interaction that associates a view with the rendering process.

