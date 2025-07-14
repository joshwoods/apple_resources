

- Image Playground
- ImageCreator
-  ImageCreator.Error 

Enumeration

# ImageCreator.Error

Errors that can occur during the image generation process.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
enum Error
```

## Topics

### Getting the error codes

case notSupported

An error that indicates the device doesn’t support image generation.

case unavailable

An error that indicates image creation is currently unavailable.

case creationCancelled

An error that occurs in response to cancellation of the parent task.

case faceInImageTooSmall

An error that indicates the system cannot use one of the source images because the face in it is too small.

case unsupportedLanguage

An error that indicates the input text uses an unsupported language.

case unsupportedInputImage

An error that indicates the system cannot use one of the specified source images.

case backgroundCreationForbidden

An error that indicates the app is hidden or in the background.

case creationFailed

An error that indicates a general failure occurred during image creation.

### Getting error-related information

var errorUserInfo: [String : Any]

The user-info dictionary.

static var errorDomain: String

The domain of the error.

### Operators

static func == (ImageCreator.Error, ImageCreator.Error) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias AllCases

A type that can represent a collection of all values of this type.

### Type Properties

static var allCases: [ImageCreator.Error]

A collection of all values of this type.

### Default Implementations

CustomNSError Implementations

Equatable Implementations

Error Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- CaseIterable
- Copyable
- CustomNSError
- Equatable
- Error
- Hashable
- LocalizedError
- Sendable

## See Also

### Generating images

func images(for: [ImagePlaygroundConcept], style: ImagePlaygroundStyle, limit: Int) -> some AsyncSequence&lt;ImageCreator.CreatedImage, any Error> 

Starts the creation of images based on the description and style information you provide.

let availableStyles: [ImagePlaygroundStyle]

The set of styles you can apply to the images you create.

struct CreatedImage

A structure that stores a programmatically generated image.

