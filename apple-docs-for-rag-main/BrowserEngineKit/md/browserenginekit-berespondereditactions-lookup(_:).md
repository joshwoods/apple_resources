

- BrowserEngineKit
- BEResponderEditActions
-  lookup(\_:) 

Instance Method

# lookup(\_:)

Presents a dictionary definition for the selected content.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
optional func lookup(_ sender: Any?)
```

## Parameters 

`sender`  

The object calling this method.

## Overview

To present the standard operating system UI for showing a dictionary definition, call showDictionary(forTextInContext:definingTextInRange:from:) in your implementation of this method.

## See Also

### Defining and sharing text

func share(Any?)

Presents UI for sharing the selected text.

