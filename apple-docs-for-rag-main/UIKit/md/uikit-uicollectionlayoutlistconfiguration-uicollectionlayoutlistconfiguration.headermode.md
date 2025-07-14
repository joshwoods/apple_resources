

- UIKit
- UICollectionLayoutListConfiguration
-  UICollectionLayoutListConfiguration.HeaderMode 

Enumeration

# UICollectionLayoutListConfiguration.HeaderMode

Constants that describe the list’s header mode.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
enum HeaderMode
```

## Topics

### Header modes

case none

No headers are shown.

case supplementary

A header mode that uses supplementary views to show headers.

case firstItemInSection

A header mode that styles the first item in a section as a header.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Configuring headers and footers

var headerMode: UICollectionLayoutListConfiguration.HeaderMode

The type of header to use for the list.

var footerMode: UICollectionLayoutListConfiguration.FooterMode

The type of footer to use for the list.

enum FooterMode

Constants that describe the list’s footer mode.

var headerTopPadding: CGFloat?

The amount of padding above each section header.

