

- SwiftUI
- ShaderLibrary
-  subscript(dynamicMember:) 

Type Subscript

# subscript(dynamicMember:)

Returns a new shader function representing the stitchable MSL function called `name` in the default shader library.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
static subscript(dynamicMember name: String) -> ShaderFunction { get }
```

## Overview

Typically this subscript is used implicitly via the dynamic member syntax, for example:

let fn = ShaderLibrary.myFunction

which creates a reference to the MSL function called `myFunction()`.

