

- Core Foundation
- CFString
-  External String Encodings 

API Collection

# External String Encodings

`CFStringEncoding` constants for encodings that may be supported by CFString.

## Overview

See the `CFStringEncodingExt.h` header file for the most current list of external string encodings and for more details.

## Topics

### Constants

case macJapanese

case macChineseTrad

case macKorean

case macArabic

case macHebrew

case macGreek

case macCyrillic

case macDevanagari

case macGurmukhi

case macGujarati

case macOriya

case macBengali

case macTamil

case macTelugu

case macKannada

case macMalayalam

case macSinhalese

case macBurmese

case macKhmer

case macThai

case macLaotian

case macGeorgian

case macArmenian

case macChineseSimp

case macTibetan

case macMongolian

case macEthiopic

case macCentralEurRoman

case macVietnamese

case macExtArabic

case macSymbol

case macDingbats

case macTurkish

case macCroatian

case macIcelandic

case macRomanian

case macCeltic

case macGaelic

case macFarsi

Like MacArabic but uses Farsi digits.

case macUkrainian

case macInuit

case macVT100

VT100102 font from Comm Toolbox: Latin-1 repertoire + box drawing etc.

case macHFS

Meta-value, should never appear in a table.

case isoLatin2

ISO 8859-2.

case isoLatin3

ISO 8859-3.

case isoLatin4

ISO 8859-4.

case isoLatinCyrillic

ISO 8859-5.

case isoLatinArabic

ISO 8859-6, =ASMO 708, =DOS CP 708.

case isoLatinGreek

ISO 8859-7.

case isoLatinHebrew

ISO 8859-8.

case isoLatin5

ISO 8859-9.

case isoLatin6

ISO 8859-10.

case isoLatinThai

ISO 8859-11.

case isoLatin7

ISO 8859-13.

case isoLatin8

ISO 8859-14.

case isoLatin9

ISO 8859-15.

case isoLatin10

ISO 8859-16.

case dosLatinUS

Code page 437.

case dosGreek

Code page 737 (formerly code page 437G).

case dosBalticRim

Code page 775.

case dosLatin1

Code page 850, “Multilingual”.

case dosGreek1

Code page 851.

case dosLatin2

Code page 852, Slavic.

case dosCyrillic

Code page 855, IBM Cyrillic.

case dosTurkish

Code page 857, IBM Turkish.

case dosPortuguese

Code page 860.

case dosIcelandic

Code page 861.

case dosHebrew

Code page 862.

case dosCanadianFrench

Code page 863.

case dosArabic

Code page 864.

case dosNordic

Code page 865.

case dosRussian

Code page 866.

case dosGreek2

Code page 869, IBM Modern Greek.

case dosThai

Code page 874, also for Windows.

case dosJapanese

Code page 932, also for Windows.

case dosChineseSimplif

Code page 936, also for Windows.

case dosKorean

Code page 949, also for Windows; Unified Hangul Code.

case dosChineseTrad

Code page 950, also for Windows.

case windowsLatin2

Code page 1250, Central Europe.

case windowsCyrillic

Code page 1251, Slavic Cyrillic.

case windowsGreek

Code page 1253.

case windowsLatin5

Code page 1254, Turkish.

case windowsHebrew

Code page 1255.

case windowsArabic

Code page 1256.

case windowsBalticRim

Code page 1257.

case windowsVietnamese

Code page 1258.

case windowsKoreanJohab

Code page 1361, for Windows NT.

case ANSEL

ANSEL (ANSI Z39.47).

case JIS_X0201_76

case JIS_X0208_83

case JIS_X0208_90

case JIS_X0212_90

case JIS_C6226_78

case shiftJIS_X0213

Shift-JIS format encoding of JIS X0213 planes 1 and 2.

case shiftJIS_X0213_MenKuTen

JIS X0213 in plane-row-column notation.

case GB_2312_80

case GBK_95

Annex to GB 13000-93; for Windows 95.

case GB_18030_2000

case KSC_5601_87

Same as KSC 5601-92 without Johab annex.

case ksc_5601_92_Johab

KSC 5601-92 Johab annex.

case CNS_11643_92_P1

CNS 11643-1992 plane 1.

case CNS_11643_92_P2

CNS 11643-1992 plane 2.

case CNS_11643_92_P3

CNS 11643-1992 plane 3 (was plane 14 in 1986 version).

case ISO_2022_JP

case ISO_2022_JP_2

case ISO_2022_JP_1

RFC 2237.

case ISO_2022_JP_3

JIS X0213.

case ISO_2022_CN

case ISO_2022_CN_EXT

case ISO_2022_KR

case EUC_JP

ISO 646, 1-byte katakana, JIS 208, JIS 212.

case EUC_CN

ISO 646, GB 2312-80.

case EUC_TW

ISO 646, CNS 11643-1992 Planes 1-16.

case EUC_KR

ISO 646, KS C 5601-1987.

case shiftJIS

Plain Shift-JIS.

case KOI8_R

Russian internet standard.

case big5

Big-5 (has variants)

case macRomanLatin1

Mac OS Roman permuted to align with ISO Latin-1.

case HZ_GB_2312

HZ (RFC 1842, for Chinese mail & news).

case big5_HKSCS_1999

Big-5 with Hong Kong special char set supplement.

case VISCII

RFC 1456, Vietnamese.

case KOI8_U

RFC 2319, Ukrainian.

case big5_E

Taiwan Big-5E standard.

case nextStepJapanese

NextStep Japanese encoding.

case EBCDIC_US

basic EBCDIC-US

case EBCDIC_CP037

code page 037, extended EBCDIC (Latin-1 set) for US, Canada.

case UTF7

kTextEncodingUnicodeDefault + kUnicodeUTF7Format RFC2152.

case UTF7_IMAP

UTF-7 (IMAP folder variant) RFC3501.

static var shiftJIS_X0213_00: CFStringEncodings

Shift-JIS format encoding of JIS X0213 planes 1 and 2.

Deprecated

## See Also

### Constants

String Comparison Flags

Flags that specify how string comparisons are performed.

enum CFStringBuiltInEncodings

Encodings that are built-in on all platforms on which macOS runs.

Invalid String Encoding Flag

Special value returned from functions to indicate a string encoding that is not supported or recognized by CFString.

