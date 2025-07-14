

- Application Services
- Carbon Accessibility
- Attributes
-  kAXFocusedApplicationAttribute 

Global Variable

# kAXFocusedApplicationAttribute

macOS 10.2+

``` source
var kAXFocusedApplicationAttribute: String { get }
```

## Discussion

Indicates the application element that is currently accepting keyboard input. This attribute is supported by the system-wide accessibility object to help an assistive application quickly determine the application that is accepting keyboard input. After the assistive application gets the accessibility object representing this application, it can send a message to the application asking for its focused accessibility object.

