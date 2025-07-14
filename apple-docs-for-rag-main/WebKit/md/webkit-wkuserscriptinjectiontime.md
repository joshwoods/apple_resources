

- WebKit
-  WKUserScriptInjectionTime 

Enumeration

# WKUserScriptInjectionTime

Constants for the times at which to inject script content into a webpage.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
enum WKUserScriptInjectionTime
```

## Topics

### Script-Injection Times

case atDocumentStart

A constant to inject the script after the creation of the webpage’s document element, but before loading any other content.

case atDocumentEnd

A constant to inject the script after the document finishes loading, but before loading any other subresources.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting Script Information

var source: String

The script’s source code.

var injectionTime: WKUserScriptInjectionTime

The time at which to inject the script into the webpage.

var isForMainFrameOnly: Bool

A Boolean value that indicates whether to inject the script into the main frame or all frames.

