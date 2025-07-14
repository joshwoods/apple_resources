

- JavaScriptCore
-  kJSClassAttributeNoAutomaticPrototype 

Global Variable

# kJSClassAttributeNoAutomaticPrototype

An attribute that specifies that a class doesn’t automatically generate a shared prototype for its instance objects.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var kJSClassAttributeNoAutomaticPrototype: Int { get }
```

## Discussion

Use kJSClassAttributeNoAutomaticPrototype with JSObjectSetPrototype(_:_:_:) to manage prototypes manually.

## See Also

### Constants

var kJSClassAttributeNone: Int

An attribute that specifies that a class has no special attributes.

