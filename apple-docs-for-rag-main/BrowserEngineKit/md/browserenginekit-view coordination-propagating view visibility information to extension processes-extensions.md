

- BrowserEngineKit
- View coordination
-  Propagating view visibility information to extension processes 

Article

# Propagating view visibility information to extension processes

Register the extensions that contribute to preparing your browser app’s UI.

## Overview

The operating system contains security checks to ensure that only the apps with which the person is interacting may draw to the screen. In a browser with extension processes, you need to indicate whether extensions participate in preparing and rendering content for a given view. Otherwise, the operating system might restrict your extensions’ access to various system resources, which might result in your browser rendering incorrectly, experiencing poor performance, or crashing.

If your browser’s extension renders content in a CALayer or hierarchy of layers, the operating system automatically propagates visibility information. Wrap the root `CALayer` in a LayerHierarchy, and send a handle to the browser app to host in a LayerHierarchyHostingView. For more information, see Hosting browser view layers in the rendering extension.

## Add a visibility propagation interaction to the view

To indicate that a web content extension or the rendering extension participates in displaying a particular view that doesn’t use a `CALayer`, your browser app requests a visibility propagation interaction from that extension’s process and attaches it to the view. For example, to use a visibility propagation interaction from the rendering extension:

```

var view: UIView

// Create and configure your view.

let visibility = renderingProcess.createVisibilityPropagationInteraction()
view.addInteraction(visibility)
```

When the rendering extension is no longer participating in the view, call the view’s removeInteraction(_:) method to remove the visibility propagation interaction.

If your extensions participate in displaying multiple views, create a separate visibility propagation interaction for each view. Don’t reuse the same interaction across multiple views.

### Display content picture-in-picture

When someone displays content from your browser app picture-in-picture, create a separate view to present the picture-in-picture content, distinct from the view that displays the content in your browser app. Create additional visibility propagation interactions for the rendering extension and web content extension, if they prepare the picture-in-picture content, and add those interactions to the view.

## See Also

### Visibility propagation

func createVisibilityPropagationInteraction() -> any UIInteraction

Returns an interaction that associates a view with the rendering process.

func createVisibilityPropagationInteraction() -> any UIInteraction

Returns an interaction that associates a view with the web content process.

