

- SwiftUI
- WidgetBundle
-  main() 

Type Method

# main()

Initializes and runs the widget bundle.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
static func main()
```

## Overview

Because you precede your WidgetBundle conformer’s declaration with the @main attribute, the system calls your widget bundle’s `main()` method to launch the widget bundle. SwiftUI provides a default implementation of the method that manages the launch process in a platform-appropriate way.

## See Also

### Running a widget bundle

init()

Creates a widget bundle using the bundle’s body as its content.

**Required**

