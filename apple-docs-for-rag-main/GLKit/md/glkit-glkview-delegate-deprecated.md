

- GLKit
- GLKView
-  delegate Deprecated

Instance Property

# delegate

The view’s delegate.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
@IBOutlet @MainActor
unowned(unsafe) var delegate: (any GLKViewDelegate)? { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

A delegate is optional. If a delegate is provided, it is called instead of calling a draw(_:) method whenever the view’s contents need to be drawn. You should either subclass the view to override the `draw` method, or provide a delegate, but not both.

