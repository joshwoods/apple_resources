

- Uniform Type Identifiers
-  System-declared uniform type identifiers 

API Collection

# System-declared uniform type identifiers

Common types that the system declares.

## Overview

Uniform type identifiers declare common types for resources an app loads, saves, or opens from other apps. Apps that use proprietary types can define them by using the system’s unified type identifiers as base types.

## Topics

### 3D content

static var threeDContent: UTType

A base type that represents 3D content.

static var usd: UTType

A type that represents Universal Scene Description content.

static var usdz: UTType

A type that represents Universal Scene Description Package content.

### Apple 3D content

static var realityFile: UTType

A type that represents a Reality Composer file.

static var sceneKitScene: UTType

A type that represents a SceneKit serialized scene.

static var arReferenceObject: UTType

A type that represents an augmented reality reference object.

### Apple file system objects

static var directory: UTType

A type that represents a file system directory, including packages and folders.

static var symbolicLink: UTType

A type that represents a symbolic link.

static var mountPoint: UTType

A type that represents a volume mount point.

static var aliasFile: UTType

A type that represents an alias file.

static var folder: UTType

A type that represents a user-browsable directory.

static var volume: UTType

A type that represents the root folder of a volume or mount point.

static var diskImage: UTType

A type that represents a data item that’s mountable as a volume.

### Apple image formats

static var heic: UTType

A type that represents High Efficiency Image Coding images.

static var heif: UTType

A type that represents High Efficiency Image File Format images.

static var livePhoto: UTType

A type that represents Live Photos.

### Apple system types

static var framework: UTType

A type that represents an Apple framework bundle.

static var applicationBundle: UTType

A type that represents a bundled app.

static var applicationExtension: UTType

A type that represents an app extension.

static var spotlightImporter: UTType

A type that represents a Spotlight metadata importer bundle.

static var quickLookGenerator: UTType

A type that represents a QuickLook preview generator bundle.

static var xpcService: UTType

A type that represents an XPC service bundle.

static var systemPreferencesPane: UTType

A type that represents a System Preferences pane.

### Application files

static var pdf: UTType

A type that represents Adobe Portable Document Format (PDF) documents.

static var rtfd: UTType

A type that represents Rich Text Format Directory documents.

static var flatRTFD: UTType

A type that represents flattened Rich Text Format Directory documents.

static var epub: UTType

A type that represents data in the electronic publication (EPUB) format.

### Audio

static var mp3: UTType

A type that represents MP3 audio.

static var aiff: UTType

A type that represents data in AIFF audio format.

static var wav: UTType

A type that represents data in Microsoft Waveform Audio File Format.

static var midi: UTType

A type that represents data in MIDI audio format.

static var playlist: UTType

A base type that represents a playlist.

static var m3uPlaylist: UTType

A type that represents an M3U or M3U8 playlist.

### Audio and video

static var quickTimeMovie: UTType

A type that represents a QuickTime movie.

static var mpeg: UTType

A type that represents an MPEG-1 or MPEG-2 movie.

static var mpeg2Video: UTType

A type that represents an MPEG-2 video.

static var mpeg2TransportStream: UTType

A type that represents data in MPEG-2 transport stream movie format.

static var mpeg4Movie: UTType

A type that represents an MPEG-4 movie.

static var mpeg4Audio: UTType

A type that represents an MPEG-4 audio layer file.

static var appleProtectedMPEG4Video: UTType

A type that represents data in Apple-protected MPEG-4 format.

static var appleProtectedMPEG4Audio: UTType

A type that represents data in Apple-protected MPEG-4 format.

static var avi: UTType

A type that represents data in AVI movie format.

### Compiled programming language sources

static var assemblyLanguageSource: UTType

A type that represents assembly language source code.

static var cHeader: UTType

A type that represents a C header file.

static var cSource: UTType

A type that represents a C source code file.

static var cPlusPlusHeader: UTType

A type that represents a C++ header file.

static var cPlusPlusSource: UTType

A type that represents a C++ source code file.

static var objectiveCPlusPlusSource: UTType

A type that represents an Objective-C++ source code file.

static var objectiveCSource: UTType

A type that represents an Objective-C source code file.

static var swiftSource: UTType

A type that represents a Swift source code file.

### Compressed archives

static var archive: UTType

A base type that represents an archive of files and directories.

static var zip: UTType

A type that represents a zip archive.

static var gzip: UTType

A type that represents a GNU zip archive.

static var bz2: UTType

A type that represents a bzip2 archive.

static var appleArchive: UTType

A type that represents an Apple archive of files and directories.

### Cryptographic files

static var pkcs12: UTType

A type that represents Public Key Cryptography Standard (PKCS) 12 data.

static var x509Certificate: UTType

A type that represents an X.509 certificate.

### Data interchange formats

static var delimitedText: UTType

A base type that represents text containing delimited values.

static var commaSeparatedText: UTType

A type that represents text containing comma-separated values.

static var tabSeparatedText: UTType

A type that represents text containing tab-separated values.

static var utf8TabSeparatedText: UTType

A type that represents UTF-8–encoded text containing tab-separated values.

static var rtf: UTType

A type that represents Rich Text Format data.

static var xml: UTType

A type that represents generic XML data.

static var yaml: UTType

A type that represents Yet Another Markup Language data.

static var json: UTType

A type that represents JavaScript Object Notation (JSON) data.

static var vCard: UTType

A type that represents a vCard file.

### Executables

static var executable: UTType

A type that represents an executable.

static var unixExecutable: UTType

A type that represents a UNIX executable.

static var exe: UTType

A type that represents a Windows executable.

### Icon images

static var ico: UTType

A type that represents Windows icon data.

static var icns: UTType

A type that represents Apple icon data.

### Images

static var png: UTType

A type that represents a PNG image.

static var gif: UTType

A type that represents a GIF image.

static var jpeg: UTType

A type that represents a JPEG image.

static var webP: UTType

A type that represents a WebP image.

static var tiff: UTType

A type that represents a TIFF image.

static var bmp: UTType

A type that represents a Windows bitmap image.

static var svg: UTType

A type that represents a scalable vector graphics (SVG) image.

static var rawImage: UTType

A base type that represents a raw image format that you use in digital photography.

### Internet-specific

static var html: UTType

A type that represents any version of HTML.

static var webArchive: UTType

A type that represents WebKit web archive data.

static var internetLocation: UTType

A base type that represents an Apple internet location file.

static var internetShortcut: UTType

A type that represents a Microsoft internet shortcut file.

### Property lists

static var propertyList: UTType

A base type that represents a property list.

static var xmlPropertyList: UTType

A type that represents an XML property list.

static var binaryPropertyList: UTType

A type that represents a binary property list.

### Shazam

static var shazamSignature: UTType

A type that represents a signature.

static var shazamCustomCatalog: UTType

A type that represents a custom catalog.

### Scripted programming language sources

static var script: UTType

A base type that represents any scripting language source.

static var appleScript: UTType

A type that represents an AppleScript text-based script.

static var javaScript: UTType

A type that represents JavaScript source code.

static var osaScript: UTType

A type that represents an Open Scripting Architecture binary script.

static var osaScriptBundle: UTType

A type that represents an Open Scripting Architecture script bundle.

static var makefile: UTType

A type that represents a Makefile.

static var shellScript: UTType

A base type that represents a shell script.

static var pythonScript: UTType

A type that represents a Python script.

static var rubyScript: UTType

A type that represents a Ruby script.

static var perlScript: UTType

A type that represents a Perl script.

static var phpScript: UTType

A type that represents a PHP script.

### Text files

static var text: UTType

A base type that represents all text-encoded data, including text with markup.

static var plainText: UTType

A type that represents text with no markup and an unspecified encoding.

static var utf8PlainText: UTType

A type that represents plain text encoded as UTF-8.

static var utf16PlainText: UTType

A type that represents plain text encoded as UTF-16 in native byte order with an optional bill of materials.

static var utf16ExternalPlainText: UTType

A type that represents plain text encoded as UTF-16 with an optional bill of materials.

### URLs

static var url: UTType

A type that represents a URL.

static var fileURL: UTType

A type that represents a URL to a file in the file system.

static var urlBookmarkData: UTType

A type that represents a URL bookmark.

### Apple system base types

static var item: UTType

A generic base type for most objects, such as files or directories.

static var content: UTType

A base type that represents anything containing user-viewable content.

static var compositeContent: UTType

A base type that represents a content format supporting mixed embedded content.

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

### Application base types

static var spreadsheet: UTType

A base type that represents a spreadsheet document.

static var presentation: UTType

A base type that represents a presentation document.

static var database: UTType

A base type that represents a database store.

static var message: UTType

A base type that represents a message.

static var contact: UTType

A base type that represents contact information.

static var calendarEvent: UTType

A base type that represents a calendar event.

static var toDoItem: UTType

A type that represents a to-do item.

static var emailMessage: UTType

A type that represents an email message.

static var font: UTType

A base type that represents a font.

### Image, audio, and video base types

static var image: UTType

A base type that represents image data.

static var audio: UTType

A type that represents audio that doesn’t contain video.

static var audiovisualContent: UTType

A base type that represents data that contains video content that may or may not also include audio.

static var movie: UTType

A base type representing media formats that may contain both video and audio.

static var video: UTType

A type that represents video that doesn’t contain audio.

### Tag classes

static var filenameExtension: UTTagClass

A type property that returns the tag class used to map a type to a filename extension.

static var mimeType: UTTagClass

A type property that returns the tag class used to map a type to a MIME type.

## See Also

### Essentials

Defining file and data types for your app

Declare uniform type identifiers to support your app’s proprietary data formats.

