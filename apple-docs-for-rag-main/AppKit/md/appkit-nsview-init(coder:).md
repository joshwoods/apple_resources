

- AppKit
- NSView
-  init(coder:) 

Initializer

# init(coder:)

Initializes a view using from data in the specified coder object.

macOS

``` source
@MainActor
init?(coder: NSCoder)
```

## Parameters 

`coder`  

The coder object that contains the view’s configuration details.

## Return Value

An initialized view or `nil` if AppKit couldn’t create the object.

## See Also

### Creating a view object

init(frame: NSRect)

Initializes and returns a newly allocated `NSView` object with a specified frame rectangle.

func prepareForReuse()

Restores the view to an initial state so that it can be reused.

