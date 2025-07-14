

- UIKit
-  UIImageReader 

Structure

# UIImageReader

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOSwatchOS 10.0+

``` source
struct UIImageReader
```

## Topics

### Structures

struct Configuration

The properties that a reader uses to decode images.

### Initializers

init(configuration: UIImageReader.Configuration)

### Instance Properties

var configuration: UIImageReader.Configuration

### Instance Methods

func image(contentsOf: URL) async -> UIImage?

func image(contentsOf: URL) -> UIImage?

func image(data: Data) async -> UIImage?

func image(data: Data) -> UIImage?

### Type Properties

static let `default`: UIImageReader

## See Also

### Creating and initializing image objects

init?(contentsOfFile: String)

Initializes and returns the image object with the contents of the specified file.

init?(data: Data)

Initializes and returns the image object with the specified data.

init?(data: Data, scale: CGFloat)

Initializes and returns the image object with the specified data and scale factor.

init(cgImage: CGImage)

Initializes and returns the image object with the specified Quartz image reference.

init(cgImage: CGImage, scale: CGFloat, orientation: UIImage.Orientation)

Initializes and returns an image object with the specified scale and orientation factors.

init(ciImage: CIImage)

Initializes and returns an image object with the specified Core Image object.

init(ciImage: CIImage, scale: CGFloat, orientation: UIImage.Orientation)

Initializes and returns an image object with the specified Core Image object and properties.

