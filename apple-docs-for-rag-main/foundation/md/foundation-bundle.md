

- Foundation
-  Bundle 

Class

# Bundle

A representation of the code and resources stored in a bundle directory on disk.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class Bundle
```

## Overview

Apple uses bundles to represent apps, frameworks, plug-ins, and many other specific types of content. Bundles organize their contained resources into well-defined subdirectories, and bundle structures vary depending on the platform and the type of the bundle. By using a bundle object, you can access a bundle’s resources without knowing the structure of the bundle. The bundle object provides a single interface for locating items, taking into account the bundle structure, user preferences, available localizations, and other relevant factors.

Any executable can use a bundle object to locate resources, either inside an app’s bundle or in a known bundle located elsewhere. You don’t use a bundle object to locate files in a container directory or in other parts of the file system.

The general pattern for using a bundle object is as follows:

1.  Create a bundle object for the intended bundle directory.

2.  Use the methods of the bundle object to locate or load the needed resource.

3.  Use other system APIs to interact with the resource.

Some types of frequently used resources can be located and opened without a bundle. For example, when loading images, you store images in asset catalogs and load them using the init(named:) methods of UIImage or NSImage. Similarly, for string resources, you use NSLocalizedString to load individual strings instead of loading the entire `.strings` file yourself.

Note

Unlike some other Foundation classes with corresponding Core Foundation names (such as NSString and CFString), Bundle objects cannot be cast to doc://com.apple.documentation/documentation/corefoundation/cfbundle-s0a references. If you need functionality provided by doc://com.apple.documentation/documentation/corefoundation/cfbundle-s0a, you can still create a doc://com.apple.documentation/documentation/corefoundation/cfbundle-s0a and use the doc://com.apple.documentation/documentation/corefoundation/cfbundle-s0a API. See Toll-Free Bridging for more information.

### Finding and Opening a Bundle

Before you can locate a resource, you must first specify which bundle contains it. The Bundle class has many constructors, but the one you use most often is main. The main bundle represents the bundle directory that contains the currently executing code. So for an app, the main bundle object gives you access to the resources that shipped with your app.

If your app interacts directly with plug-ins, frameworks, or other bundled content, you can use other methods of this class to create appropriate bundle objects. You can always create bundle objects from a known URL or path, but other methods make it easier to access bundles your app is already using. For example, if you link to a framework, you can use the init(for:) method to locate the framework bundle based on a class defined in that framework.

- Swift
- Objective-C

```
// Get the app's main bundle
let mainBundle = Bundle.main

// Get the bundle containing the specified private class.
let myBundle = Bundle(for: NSClassFromString("MyPrivateClass")!)
```

```
// Get the app's main bundle
NSBundle *main = [NSBundle mainBundle];

// Get the bundle containing the specified private class.
NSBundle *myBundle = [NSBundle bundleForClass:[MyPrivateClass class]];
```

### Locating Resources in a Bundle

You use Bundle objects to obtain the location of specific resources inside the bundle. When looking for resources, you provide the name of the resource and its type at a minimum. For resources in a specific subdirectory, you can also specify that directory. After locating the resource, the bundle routines return a path string or URL that you can use to open the file.

Listing 2. Locating a single resource in a bundle

```
NSBundle *main = [NSBundle mainBundle];
NSString *resourcePath = [main pathForResource:@"Seagull" ofType:@"jpg"];
```

Bundle objects follow a specific search pattern when looking for resources on disk. Global resources—that is, resources not in a language-specific `.lproj` directory—are returned first, followed by region- and language-specific resources. This search pattern means that the bundle looks for resources in the following order:

1.  Global (nonlocalized) resources

2.  Region-specific localized resources (based on the user’s region preferences)

3.  Language-specific localized resources (based on the user’s language preferences)

4.  Development language resources (as specified by the CFBundleDevelopmentRegion key in the bundle’s Info.plist file)

Because global resources take precedence over language-specific resources, you should never include both a global and localized version of a given resource in your app. When a global version of a resource exists, language-specific versions are never returned. The reason for this precedence is performance. If localized resources were searched first, the bundle object might waste time searching for a nonexistent localized resource before returning the global resource.

Important

Bundle objects always consider case when searching for resource files, even on file systems that support case-insensitive filenames. Always make sure that you specify filenames with case sensitivity in mind.

When locating resource files, the bundle object automatically considers many standard filename modifiers when determining which file to return. Resources may be tagged for a specific device (`~iphone`, `~ipad`) or for a specific screen resolution (`@2x`, `@3x`). Do not include these modifiers when specifying the name of the resource you want. The bundle object selects the file that is most appropriate for the underlying device. For more information, see App Icons on iPhone, iPad and Apple Watch.

### Understanding Bundle Structures

Bundle structures vary depending on the target platform and the type of bundle you are building. The Bundle class hides this underlying structure in most (but not all) cases. Many of the methods you use to load resources from a bundle automatically locate the appropriate starting directory and look for resources in known places. You can also use the methods and properties of this class to get the location of known bundle directories and to retrieve resources specifically from those directories.

For information about the bundle structure of iOS and macOS apps, see Bundle Programming Guide. For information about the structure of framework bundles, see Framework Programming Guide. For information about the structure of macOS plug-ins, see Code Loading Programming Topics.

## Topics

### Getting Standard Bundle Objects

class var main: Bundle

Returns the bundle object that contains the current executable.

class var allFrameworks: [Bundle]

Returns an array of all of the application’s bundles that represent frameworks.

class var allBundles: [Bundle]

Returns an array of all the application’s non-framework bundles.

### Creating and Initializing a Bundle

init(for: AnyClass)

Returns the `NSBundle` object with which the specified class is associated.

init?(identifier: String)

Returns the `NSBundle` instance that has the specified bundle identifier.

convenience init?(url: URL)

Returns an `NSBundle` object initialized to correspond to the specified file URL.

init?(path: String)

Returns an `NSBundle` object initialized to correspond to the specified directory.

### Loading Nib Files

func loadNibNamed(String, owner: Any?, options: [UINib.OptionsKey : Any]?) -> [Any]?

Unarchives the contents of a nib file located in the receiver’s bundle.

func loadNibNamed(NSNib.Name, owner: Any?, topLevelObjects: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) -> Bool

Loads a nib from the bundle with the specified file name and owner.

### Finding Resource Files

func url(forResource: String?, withExtension: String?, subdirectory: String?) -> URL?

Returns the file URL for the resource file identified by the specified name and extension and residing in a given bundle directory.

func url(forResource: String?, withExtension: String?) -> URL?

Returns the file URL for the resource identified by the specified name and file extension.

func urls(forResourcesWithExtension: String?, subdirectory: String?) -> [URL]?

Returns an array of file URLs for all resources identified by the specified file extension and located in the specified bundle subdirectory.

func url(forResource: String?, withExtension: String?, subdirectory: String?, localization: String?) -> URL?

Returns the file URL for the resource identified by the specified name and file extension, located in the specified bundle subdirectory, and limited to global resources and those associated with the specified localization.

func urls(forResourcesWithExtension: String?, subdirectory: String?, localization: String?) -> [URL]?

Returns an array containing the file URLs for all bundle resources having the specified filename extension, residing in the specified resource subdirectory, and limited to global resources and those associated with the specified localization.

class func url(forResource: String?, withExtension: String?, subdirectory: String?, in: URL) -> URL?

Creates and returns a file URL for the resource with the specified name and extension in the specified bundle.

class func urls(forResourcesWithExtension: String?, subdirectory: String?, in: URL) -> [URL]?

Returns an array containing the file URLs for all bundle resources having the specified filename extension, residing in the specified resource subdirectory, within the specified bundle.

func path(forResource: String?, ofType: String?) -> String?

Returns the full pathname for the resource identified by the specified name and file extension.

func path(forResource: String?, ofType: String?, inDirectory: String?) -> String?

Returns the full pathname for the resource identified by the specified name and file extension and located in the specified bundle subdirectory.

func path(forResource: String?, ofType: String?, inDirectory: String?, forLocalization: String?) -> String?

Returns the full pathname for the resource identified by the specified name and file extension, located in the specified bundle subdirectory, and limited to global resources and those associated with the specified localization.

func paths(forResourcesOfType: String?, inDirectory: String?) -> [String]

Returns an array containing the pathnames for all bundle resources having the specified filename extension and residing in the resource subdirectory.

func paths(forResourcesOfType: String?, inDirectory: String?, forLocalization: String?) -> [String]

Returns an array containing the file for all bundle resources having the specified filename extension, residing in the specified resource subdirectory, and limited to global resources and those associated with the specified localization.

class func path(forResource: String?, ofType: String?, inDirectory: String) -> String?

Returns the full pathname for the resource file identified by the specified name and extension and residing in a given bundle directory.

class func paths(forResourcesOfType: String?, inDirectory: String) -> [String]

Returns an array containing the pathnames for all bundle resources having the specified extension and residing in the bundle directory at the specified path.

### Finding Image Resources

func urlForImageResource(NSImage.Name) -> URL?

Returns the location of the specified image resource as an NSURL.

func pathForImageResource(NSImage.Name) -> String?

Returns the location of the specified image resource file.

func image(forResource: NSImage.Name) -> NSImage?

Returns an `NSImage` instance associated with the specified name, which can be backed by multiple files representing different resolution versions of the image.

### Finding Sound Resources

func path(forSoundResource: NSSound.Name) -> String?

Returns the location of the specified sound resource file.

### Fetching Localized Strings

func localizedString(forKey: String, value: String?, table: String?) -> String

Returns a localized version of the string designated by the specified key and residing in the specified table.

### Fetching Context Help Resources

func contextHelp(forKey: NSHelpManager.ContextHelpKey) -> NSAttributedString?

Returns the context-sensitive help for the specified key from the bundle’s help file.

### Getting the Standard Bundle Directories

var resourceURL: URL?

The file URL of the bundle’s subdirectory containing resource files.

var executableURL: URL?

The file URL of the receiver’s executable file.

var privateFrameworksURL: URL?

The file URL of the bundle’s subdirectory containing private frameworks.

var sharedFrameworksURL: URL?

The file URL of the receiver’s subdirectory containing shared frameworks.

var builtInPlugInsURL: URL?

The file URL of the receiver’s subdirectory containing plug-ins.

func url(forAuxiliaryExecutable: String) -> URL?

Returns the file URL of the executable with the specified name in the receiver’s bundle.

var sharedSupportURL: URL?

The file URL of the bundle’s subdirectory containing shared support files.

var appStoreReceiptURL: URL?

The file URL for the bundle’s App Store receipt.

Deprecated

var resourcePath: String?

The full pathname of the bundle’s subdirectory containing resources.

var executablePath: String?

The full pathname of the receiver’s executable file.

var privateFrameworksPath: String?

The full pathname of the bundle’s subdirectory containing private frameworks.

var sharedFrameworksPath: String?

The full pathname of the bundle’s subdirectory containing shared frameworks.

var builtInPlugInsPath: String?

The full pathname of the receiver’s subdirectory containing plug-ins.

func path(forAuxiliaryExecutable: String) -> String?

Returns the full pathname of the executable with the specified name in the receiver’s bundle.

var sharedSupportPath: String?

The full pathname of the bundle’s subdirectory containing shared support files.

### Getting Bundle Information

var bundleURL: URL

The full URL of the receiver’s bundle directory.

var bundlePath: String

The full pathname of the receiver’s bundle directory.

var bundleIdentifier: String?

The receiver’s bundle identifier.

var infoDictionary: [String : Any]?

A dictionary, constructed from the bundle’s `Info.plist` file, that contains information about the receiver.

func object(forInfoDictionaryKey: String) -> Any?

Returns the value associated with the specified key in the receiver’s information property list.

### Getting Localization Information

var localizations: [String]

A list of all the localizations contained in the bundle.

var preferredLocalizations: [String]

An ordered list of preferred localizations contained in the bundle.

var developmentLocalization: String?

The localization for the development language.

var localizedInfoDictionary: [String : Any]?

A dictionary with the keys from the bundle’s localized property list.

class func preferredLocalizations(from: [String]) -> [String]

Returns one or more localizations from the specified list that a bundle object would use to locate resources for the current user.

class func preferredLocalizations(from: [String], forPreferences: [String]?) -> [String]

Returns locale identifiers for which a bundle would provide localized content, given a specified list of candidates for a user’s language preferences.

### Managing Preservation Priority for On Demand Resources

func setPreservationPriority(Double, forTags: Set&lt;String>)

A hint to the system of the relative order for purging tagged sets of resources in the bundle.

func preservationPriority(forTag: String) -> Double

Returns the current preservation priority for the specified tag.

### Getting Classes from a Bundle

func classNamed(String) -> AnyClass?

Returns the `Class` object for the specified name.

var principalClass: AnyClass?

The bundle’s principal class.

class let didLoadNotification: NSNotification.Name

A notification that lets observers know when classes are dynamically loaded.

let NSLoadedClasses: String

A constant used as a key for the `userInfo` dictionary of a didLoadNotification notification that corresponds to an array of names of each class that was loaded.

### Loading Code from a Bundle

var executableArchitectures: [NSNumber]?

An array of numbers indicating the architecture types supported by the bundle’s executable.

func preflight() throws

Returns a Boolean value indicating whether the bundle’s executable code could be loaded successfully.

func load() -> Bool

Dynamically loads the bundle’s executable code into a running program, if the code has not already been loaded.

func loadAndReturnError() throws

Loads the bundle’s executable code and returns any errors.

func unload() -> Bool

Unloads the code associated with the receiver.

var isLoaded: Bool

The load status of a bundle.

Mach-O Architecture

Constants that describe the CPU types that a bundle’s executable code supports.

### Errors

var NSExecutableErrorMinimum: Int

The beginning of the range of error codes reserved for errors related to executable files.

var NSExecutableNotLoadableError: Int

The executable type isn’t loadable in the current process.

var NSExecutableArchitectureMismatchError: Int

The executable doesn’t provide an architecture compatible with the current process.

var NSExecutableRuntimeMismatchError: Int

The executable has Objective-C runtime information that’s incompatible with the current process.

var NSExecutableLoadError: Int

Executable cannot be loaded for an otherwise-unspecified reason.

var NSExecutableLinkError: Int

The executable failed due to linking issues.

var NSExecutableErrorMaximum: Int

The end of the range of error codes reserved for errors related to executable files.

### Instance Methods

func loadAppleScriptObjectiveCScripts()

func localizedString(forKey: String, value: String?, table: String?, localizations: [Locale.Language]) -> String

Look up a localized string given a list of available languages.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

