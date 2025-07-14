

- UIKit
-  UIBarMetrics 

Enumeration

# UIBarMetrics

Constants to specify metrics to use for appearance.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum UIBarMetrics
```

## Topics

### Constants

case `default`

Specifies default metrics for the device.

case compact

Specifies metrics when using the phone idiom.

case defaultPrompt

Specifies default metrics for the device for bars with the prompt property, such as UINavigationBar and UISearchBar.

case compactPrompt

Specifies metrics for bars with the prompt property when using the phone idiom, such as UINavigationBar and UISearchBar.

static var landscapePhone: UIBarMetrics

Specifies metrics for landscape orientation using the phone idiom.

Deprecated

static var landscapePhonePrompt: UIBarMetrics

Specifies metrics for landscape orientation using the phone idiom for bars with the prompt property, such as UINavigationBar and UISearchBar.

Deprecated

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

### Constants

enum UIBarPosition

Constants to identify the position of a bar.

