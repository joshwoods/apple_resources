

- Core Services
- Carbon Core
-  Unicode Utilities Deprecated

API Collection

# Unicode Utilities

Work with Unicode text.

Deprecated

Many APIs that use text encodings other than Unicode are deprecated in macOS 10. Instead, use APIs that support Unicode, such as those provided by the Foundation and Core Foundation frameworks. For more information, see String Programming Guide.

## Topics

### Inputting Unicode Text

func UCKeyTranslate(UnsafePointer&lt;UCKeyboardLayout>!, UInt16, UInt16, UInt32, UInt32, OptionBits, UnsafeMutablePointer&lt;UInt32>!, Int, UnsafeMutablePointer&lt;Int>!, UnsafeMutablePointer&lt;UniChar>!) -> OSStatus

Converts a combination of a virtual key code, a modifier key state, and a dead-key state into a string of one or more Unicode characters.

### Comparing Unicode Strings

func UCCreateCollator(LocaleRef!, LocaleOperationVariant, UCCollateOptions, UnsafeMutablePointer&lt;CollatorRef?>!) -> OSStatus

Creates an object encapsulating locale and collation information, for the purpose of performing Unicode string comparison.

func UCCompareText(CollatorRef!, UnsafePointer&lt;UniChar>!, Int, UnsafePointer&lt;UniChar>!, Int, UnsafeMutablePointer&lt;DarwinBoolean>!, UnsafeMutablePointer&lt;Int32>!) -> OSStatus

Uses locale-specific collation information to compare Unicode strings.

func UCGetCollationKey(CollatorRef!, UnsafePointer&lt;UniChar>!, Int, Int, UnsafeMutablePointer&lt;Int>!, UnsafeMutablePointer&lt;UCCollationValue>!) -> OSStatus

Uses locale-specific collation information to generate a collation key for a Unicode string.

func UCCompareCollationKeys(UnsafePointer&lt;UCCollationValue>!, Int, UnsafePointer&lt;UCCollationValue>!, Int, UnsafeMutablePointer&lt;DarwinBoolean>!, UnsafeMutablePointer&lt;Int32>!) -> OSStatus

Uses collation keys to compare Unicode strings.

func UCDisposeCollator(UnsafeMutablePointer&lt;CollatorRef?>!) -> OSStatus

Disposes a collator object.

func UCCompareTextDefault(UCCollateOptions, UnsafePointer&lt;UniChar>!, Int, UnsafePointer&lt;UniChar>!, Int, UnsafeMutablePointer&lt;DarwinBoolean>!, UnsafeMutablePointer&lt;Int32>!) -> OSStatus

Uses the default system locale to compare Unicode strings.

func UCCompareTextNoLocale(UCCollateOptions, UnsafePointer&lt;UniChar>!, Int, UnsafePointer&lt;UniChar>!, Int, UnsafeMutablePointer&lt;DarwinBoolean>!, UnsafeMutablePointer&lt;Int32>!) -> OSStatus

Uses a fixed, locale-insensitive order to compare Unicode strings.

### Data Types

typealias CollatorRef

Refers to an opaque object that encapsulates locale and collation information for the purpose of performing Unicode string comparison.

typealias TextBreakLocatorRef

Refers to an opaque object that encapsulates locale and text-break information for the purpose of finding boundaries in Unicode text.

typealias UCCollationValue

Specifies a Unicode collation key.

struct UCKeyboardLayout

Provides header data for a `'uchr'` resource.

struct UCKeyboardTypeHeader

Specifies a range of physical keyboard types in a `'uchr'` resource.

typealias UCKeyCharSeq

Specifies the output of a dead-key state in a `'uchr'` resource.

struct UCKeyLayoutFeatureInfo

Specifies the longest possible output string to be produced by the current `'uchr'` resource.

struct UCKeyModifiersToTableNum

Maps a modifier key combination to a particular key-code-to-character table number in a `'uchr'` resource.

typealias UCKeyOutput

Specifies values in key-code-to-character tables in a `'uchr'` resource.

struct UCKeySequenceDataIndex

Contains offsets to a list of character sequences for a `'uchr'` resource.

struct UCKeyStateEntryRange

Maps from a dead-key state to either the resultant Unicode character(s) or the new dead key state produced when the current state is terminated by a given character key for a `'uchr'` resource.

struct UCKeyStateEntryTerminal

Maps from a dead-key state to the Unicode character(s) produced when that state is terminated by a given character key for a `'uchr'` resource.

struct UCKeyStateRecord

Determines dead-key state transitions in a `'uchr'` resource.

struct UCKeyStateRecordsIndex

Provides a count of, and offsets to, dead-key state records in a `'uchr'` resource.

struct UCKeyStateTerminators

Lists the default terminators for each dead-key state handled by a `'uchr'` resource.

struct UCKeyToCharTableIndex

Provides a count of, and offsets to, key-code-to-character tables in a `'uchr'` resource.

### Constants

Fixed Ordering Scheme

Specifies to use the fixed ordering scheme.

Fixed Ordering Masks 1

Set and test the `UCCollateOptions` field that specifies a fixed ordering scheme.

Fixed Ordering Masks 2

Test the `UCCollateOptions` field that specifies a fixed ordering scheme.

Key Actions

Indicate the current key action.

Key Format Codes

Indicate a structure format used in a `'uchr'` resource.

Key Output Index Masks

Test the bits in `UCKeyOutput` values.

Key State Entry Formats

Indicate the format for dead-key state records.

Key Translation Options Flag

Indicates the dead-key processing state.

Key Translation Options Mask

Specifies the mask for the bit that controls dead-key processing state.

Operation Class

Identifies collation as a class of Unicode utility operations.

Standard Options Mask

Specifies standard options for Unicode string comparison.

typealias UCCollateOptions

Specifies options for Unicode string comparison.

typealias UCTextBreakOptions

Specifies options for locating boundaries in Unicode text.

typealias UCTextBreakType

Specifies kinds of text boundaries.

Text Boundary Operation Class

Identifies the class of Unicode utility operations that find text boundaries.

