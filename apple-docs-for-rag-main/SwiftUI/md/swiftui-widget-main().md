

- SwiftUI
- Widget
-  main() 

Type Method

# main()

Initializes and runs the widget.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
static func main()
```

## Overview

Because you precede your Widget conformer’s declaration with the @main attribute, the system calls your widget’s `main()` method to launch the widget. SwiftUI provides a default implementation of the method that manages the launch process in a platform-appropriate way.

## See Also

### Running a widget

init()

Creates a widget using `body` as its content.

**Required**

