

- BrowserEngineKit
- BETextInput
-  insert(\_:) 

Instance Method

# insert(\_:)

Inserts a `textSuggestion` in response to a user suggestion selection

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func insert(_ textSuggestion: BETextSuggestion)
```

**Required**

## Parameters 

`textSuggestion`  

The suggestion to insert.

## Mentioned in 

Integrating custom browser text views with UIKit

## Discussion

Inserts suggested text.

## Overview

The system calls this method to suggest insertions into the text view, for example AutoFill credentials.

