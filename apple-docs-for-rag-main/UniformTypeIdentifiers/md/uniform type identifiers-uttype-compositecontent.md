

- Uniform Type Identifiers
- UTType
-  compositeContent 

Type Property

# compositeContent

A base type that represents a content format supporting mixed embedded content.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var compositeContent: UTType { get }
```

## Discussion

The identifier for this type is `public.composite-content`.

This type conforms to UTTypeContent.

## See Also

### Apple system base types

static var item: UTType

A generic base type for most objects, such as files or directories.

static var content: UTType

A base type that represents anything containing user-viewable content.

static var data: UTType

A base type that represents any sort of byte stream, including files and in-memory data.

static var resolvable: UTType

A base type that represents a resolvable reference, including symbolic links and aliases.

static var package: UTType

A base type that represents a packaged directory.

static var bundle: UTType

A base type that represents a directory that conforms to one of the bundle layouts.

static var pluginBundle: UTType

A base type that represents a bundle-based plug-in.

static var application: UTType

A base type that represents a macOS, iOS, iPadOS, watchOS, and tvOS app.

static var sourceCode: UTType

A base type that represents source code of any programming language.

static var bookmark: UTType

A base type that represents bookmark data.

static var log: UTType

A base type that represents console log data.

