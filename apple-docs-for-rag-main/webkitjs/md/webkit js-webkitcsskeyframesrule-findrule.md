

- WebKit JS
- WebKitCSSKeyframesRule
-  findRule 

# findRule

Returns the keyframe rule for the specified selector.

``` source
WebKitCSSKeyframeRule findRule (in DOMString key);
```

## Parameters 

`key`  

A selector for the rule that is either a percentage or the keyword `from` or `to`.

## Return Value

Returns the keyframe rule corresponding to the given selector if it exists.

## See Also

### Changing Rules

insertRule

Adds a keyframe rule to the collection of keyframes.

deleteRule

Removes a keyframe rule from the collection of keyframes.

