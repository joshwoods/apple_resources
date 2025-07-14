

- Core Foundation
-  CFStringEncodings 

Enumeration

# CFStringEncodings

Index type for constants used to specify external string encodings.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CFStringEncodings
```

## Topics

### Enumeration Cases

case ANSEL

ANSEL (ANSI Z39.47).

case big5

Big-5 (has variants)

case big5_E

Taiwan Big-5E standard.

case big5_HKSCS_1999

Big-5 with Hong Kong special char set supplement.

case CNS_11643_92_P1

CNS 11643-1992 plane 1.

case CNS_11643_92_P2

CNS 11643-1992 plane 2.

case CNS_11643_92_P3

CNS 11643-1992 plane 3 (was plane 14 in 1986 version).

case dosArabic

Code page 864.

case dosBalticRim

Code page 775.

case dosCanadianFrench

Code page 863.

case dosChineseSimplif

Code page 936, also for Windows.

case dosChineseTrad

Code page 950, also for Windows.

case dosCyrillic

Code page 855, IBM Cyrillic.

case dosGreek

Code page 737 (formerly code page 437G).

case dosGreek1

Code page 851.

case dosGreek2

Code page 869, IBM Modern Greek.

case dosHebrew

Code page 862.

case dosIcelandic

Code page 861.

case dosJapanese

Code page 932, also for Windows.

case dosKorean

Code page 949, also for Windows; Unified Hangul Code.

case dosLatin1

Code page 850, “Multilingual”.

case dosLatin2

Code page 852, Slavic.

case dosLatinUS

Code page 437.

case dosNordic

Code page 865.

case dosPortuguese

Code page 860.

case dosRussian

Code page 866.

case dosThai

Code page 874, also for Windows.

case dosTurkish

Code page 857, IBM Turkish.

case EBCDIC_CP037

code page 037, extended EBCDIC (Latin-1 set) for US, Canada.

case EBCDIC_US

basic EBCDIC-US

case EUC_CN

ISO 646, GB 2312-80.

case EUC_JP

ISO 646, 1-byte katakana, JIS 208, JIS 212.

case EUC_KR

ISO 646, KS C 5601-1987.

case EUC_TW

ISO 646, CNS 11643-1992 Planes 1-16.

case GBK_95

Annex to GB 13000-93; for Windows 95.

case GB_18030_2000

case GB_2312_80

case HZ_GB_2312

HZ (RFC 1842, for Chinese mail & news).

case isoLatin10

ISO 8859-16.

case isoLatin2

ISO 8859-2.

case isoLatin3

ISO 8859-3.

case isoLatin4

ISO 8859-4.

case isoLatin5

ISO 8859-9.

case isoLatin6

ISO 8859-10.

case isoLatin7

ISO 8859-13.

case isoLatin8

ISO 8859-14.

case isoLatin9

ISO 8859-15.

case isoLatinArabic

ISO 8859-6, =ASMO 708, =DOS CP 708.

case isoLatinCyrillic

ISO 8859-5.

case isoLatinGreek

ISO 8859-7.

case isoLatinHebrew

ISO 8859-8.

case isoLatinThai

ISO 8859-11.

case ISO_2022_CN

case ISO_2022_CN_EXT

case ISO_2022_JP

case ISO_2022_JP_1

RFC 2237.

case ISO_2022_JP_2

case ISO_2022_JP_3

JIS X0213.

case ISO_2022_KR

case JIS_C6226_78

case JIS_X0201_76

case JIS_X0208_83

case JIS_X0208_90

case JIS_X0212_90

case KOI8_R

Russian internet standard.

case KOI8_U

RFC 2319, Ukrainian.

case KSC_5601_87

Same as KSC 5601-92 without Johab annex.

case ksc_5601_92_Johab

KSC 5601-92 Johab annex.

case macArabic

case macArmenian

case macBengali

case macBurmese

case macCeltic

case macCentralEurRoman

case macChineseSimp

case macChineseTrad

case macCroatian

case macCyrillic

case macDevanagari

case macDingbats

case macEthiopic

case macExtArabic

case macFarsi

Like MacArabic but uses Farsi digits.

case macGaelic

case macGeorgian

case macGreek

case macGujarati

case macGurmukhi

case macHFS

Meta-value, should never appear in a table.

case macHebrew

case macIcelandic

case macInuit

case macJapanese

case macKannada

case macKhmer

case macKorean

case macLaotian

case macMalayalam

case macMongolian

case macOriya

case macRomanLatin1

Mac OS Roman permuted to align with ISO Latin-1.

case macRomanian

case macSinhalese

case macSymbol

case macTamil

case macTelugu

case macThai

case macTibetan

case macTurkish

case macUkrainian

case macVT100

VT100102 font from Comm Toolbox: Latin-1 repertoire + box drawing etc.

case macVietnamese

case nextStepJapanese

NextStep Japanese encoding.

case shiftJIS

Plain Shift-JIS.

case shiftJIS_X0213

Shift-JIS format encoding of JIS X0213 planes 1 and 2.

case shiftJIS_X0213_MenKuTen

JIS X0213 in plane-row-column notation.

case UTF7

kTextEncodingUnicodeDefault + kUnicodeUTF7Format RFC2152.

case UTF7_IMAP

UTF-7 (IMAP folder variant) RFC3501.

case VISCII

RFC 1456, Vietnamese.

case windowsArabic

Code page 1256.

case windowsBalticRim

Code page 1257.

case windowsCyrillic

Code page 1251, Slavic Cyrillic.

case windowsGreek

Code page 1253.

case windowsHebrew

Code page 1255.

case windowsKoreanJohab

Code page 1361, for Windows NT.

case windowsLatin2

Code page 1250, Central Europe.

case windowsLatin5

Code page 1254, Turkish.

case windowsVietnamese

Code page 1258.

### Initializers

init?(rawValue: CFIndex)

### Type Properties

static var shiftJIS_X0213_00: CFStringEncodings

Shift-JIS format encoding of JIS X0213 planes 1 and 2.

Deprecated

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Data Types

typealias CFStringEncoding

An integer type for constants used to specify supported string encodings in various CFString functions.

struct CFStringCompareFlags

A CFOptionFlags type for specifying options for string comparison .

struct CFStringInlineBuffer

Defines the buffer and related fields used for in-line buffer access of characters in CFString objects.

