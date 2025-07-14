

- Core Text
-  SFNT Support 

API Collection

# SFNT Support

## Topics

### Structures

struct AnchorPoint

struct AnchorPointTable

struct AnkrTable

struct BslnFormat0Part

struct BslnFormat1Part

struct BslnFormat2Part

struct BslnFormat3Part

struct BslnFormatUnion

struct BslnTable

struct FontVariation

struct JustDirectionTable

struct JustPCAction

struct JustPCActionSubrecord

struct JustPCConditionalAddAction

struct JustPCDecompositionAction

struct JustPCDuctilityAction

struct JustPCGlyphRepeatAddAction

struct JustPostcompTable

struct JustTable

struct JustWidthDeltaEntry

struct JustWidthDeltaGroup

struct KernFormatSpecificHeader

struct KernIndexArrayHeader

struct KernKerningPair

struct KernOffsetTable

struct KernOrderedListEntry

struct KernOrderedListHeader

struct KernSimpleArrayHeader

struct KernStateEntry

struct KernStateHeader

struct KernSubtableHeader

struct KernTableHeader

struct KernVersion0Header

struct KernVersion0SubtableHeader

struct KerxAnchorPointAction

struct KerxControlPointAction

struct KerxControlPointEntry

struct KerxControlPointHeader

struct KerxCoordinateAction

struct KerxFormatSpecificHeader

struct KerxIndexArrayHeader

struct KerxKerningPair

struct KerxOrderedListEntry

struct KerxOrderedListHeader

struct KerxSimpleArrayHeader

struct KerxStateEntry

struct KerxStateHeader

struct KerxSubtableHeader

struct KerxTableHeader

struct LcarCaretClassEntry

struct LcarCaretTable

struct MortChain

struct MortContextualSubtable

struct MortFeatureEntry

struct MortInsertionSubtable

struct MortLigatureSubtable

struct MortRearrangementSubtable

struct MortSpecificSubtable

struct MortSubtable

struct MortSwashSubtable

struct MortTable

struct MorxChain

struct MorxContextualSubtable

struct MorxInsertionSubtable

struct MorxLigatureSubtable

struct MorxRearrangementSubtable

struct MorxSpecificSubtable

struct MorxSubtable

struct MorxTable

struct OpbdSideValues

struct OpbdTable

struct PropLookupSegment

struct PropLookupSingle

struct PropTable

struct ROTAGlyphEntryDeprecated

struct ROTAHeaderDeprecated

struct SFNTLookupArrayHeader

struct SFNTLookupBinarySearchHeader

struct SFNTLookupFormatSpecificHeader

struct SFNTLookupSegment

struct SFNTLookupSegmentHeader

struct SFNTLookupSingle

struct SFNTLookupSingleHeader

struct SFNTLookupTable

struct SFNTLookupTrimmedArrayHeader

struct STClassTable

struct STEntryOne

struct STEntryTwo

struct STEntryZero

struct STHeader

struct STXEntryOne

struct STXEntryTwo

struct STXEntryZero

struct STXHeader

struct TrakTable

struct TrakTableData

struct TrakTableEntry

struct sfntCMapEncoding

struct sfntCMapExtendedSubHeader

struct sfntCMapHeader

struct sfntCMapSubHeader

struct sfntDescriptorHeader

struct sfntDirectory

struct sfntDirectoryEntry

struct sfntFeatureHeader

struct sfntFeatureName

struct sfntFontDescriptor

struct sfntFontFeatureSetting

struct sfntFontRunFeature

struct sfntInstance

struct sfntNameHeader

struct sfntNameRecord

struct sfntVariationAxis

struct sfntVariationHeader

struct ALMXGlyphEntryDeprecated

struct ALMXHeaderDeprecated

### Type Aliases

typealias BslnBaselineClass

typealias BslnBaselineRecord

typealias BslnTableFormat

typealias BslnTablePtr

typealias FontLanguageCode

typealias FontNameCode

typealias FontPlatformCode

typealias FontScriptCode

typealias JustPCActionType

typealias JustPCUnconditionalAddAction

typealias JustificationFlags

typealias KernArrayOffset

typealias KernKerningValue

typealias KernOffsetTablePtr

typealias KernOrderedListEntryPtr

typealias KernSubtableHeaderPtr

typealias KernSubtableInfo

typealias KernTableFormat

typealias KernTableHeaderHandle

typealias KernTableHeaderPtr

typealias KerxArrayOffset

typealias KerxOrderedListEntryPtr

typealias KerxSubtableCoverage

typealias KerxSubtableHeaderPtr

typealias KerxTableHeaderHandle

typealias KerxTableHeaderPtr

typealias LcarCaretTablePtr

typealias MortLigatureActionEntry

typealias MortSubtableMaskFlags

typealias OpbdTableFormat

typealias PropCharProperties

typealias SFNTLookupKind

typealias SFNTLookupOffset

typealias SFNTLookupTableFormat

typealias SFNTLookupTableHandle

typealias SFNTLookupTablePtr

typealias SFNTLookupValue

typealias STClass

typealias STEntryIndex

typealias STXClass

typealias STXClassTable

typealias STXEntryIndex

typealias STXStateIndex

typealias TrakValue

### Constants

var cmapFontTableTag: Int

var descriptorFontTableTag: Int

var featureFontTableTag: Int

var kANKRCurrentVersion: Int

var kAbbrevSquaredLigaturesOffSelector: Int

var kAbbrevSquaredLigaturesOnSelector: Int

var kAllCapsSelector: Int

var kAllLowerCaseSelector: Int

var kAllTypeFeaturesOffSelector: Int

var kAllTypeFeaturesOnSelector: Int

var kAllTypographicFeaturesType: Int

var kAltHalfWidthTextSelector: Int

var kAltProportionalTextSelector: Int

var kAlternateHorizKanaOffSelector: Int

var kAlternateHorizKanaOnSelector: Int

var kAlternateKanaType: Int

var kAlternateVertKanaOffSelector: Int

var kAlternateVertKanaOnSelector: Int

var kAnnotationType: Int

var kAsteriskToMultiplyOffSelector: Int

var kAsteriskToMultiplyOnSelector: Int

var kBSLNControlPointFormatNoMap: Int

var kBSLNControlPointFormatWithMap: Int

var kBSLNCurrentVersion: Int

var kBSLNDistanceFormatNoMap: Int

var kBSLNDistanceFormatWithMap: Int

var kBSLNHangingBaseline: Int

var kBSLNIdeographicCenterBaseline: Int

var kBSLNIdeographicLowBaseline: Int

var kBSLNLastBaseline: Int

var kBSLNMathBaseline: Int

var kBSLNNoBaseline: Int

var kBSLNNoBaselineOverride: Int

var kBSLNNumBaselineClasses: Int

var kBSLNRomanBaseline: Int

var kBSLNTag: Int

var kBoxAnnotationSelector: Int

var kCJKItalicRomanOffSelector: Int

var kCJKItalicRomanOnSelector: Int

var kCJKItalicRomanSelector: Int

var kCJKRomanSpacingType: Int

var kCJKSymbolAltFiveSelector: Int

var kCJKSymbolAltFourSelector: Int

var kCJKSymbolAltOneSelector: Int

var kCJKSymbolAltThreeSelector: Int

var kCJKSymbolAltTwoSelector: Int

var kCJKSymbolAlternativesType: Int

var kCJKVerticalRomanCenteredSelector: Int

var kCJKVerticalRomanHBaselineSelector: Int

var kCJKVerticalRomanPlacementType: Int

var kCTFontTableCBDT: Int

var kCTFontTableCBLC: Int

var kCTFontTableCFF2: Int

var kCTFontTableCOLR: Int

var kCTFontTableCPAL: Int

var kCTFontTableCidg: Int

var kCTFontTableFond: Int

var kCTFontTableHVAR: Int

var kCTFontTableMERG: Int

var kCTFontTableMVAR: Int

var kCTFontTableMeta: Int

var kCTFontTableSTAT: Int

var kCTFontTableSVG: Int

var kCTFontTableVVAR: Int

var kCTFontTableXref: Int

var kCanonicalCompositionOffSelector: Int

var kCanonicalCompositionOnSelector: Int

var kCaseSensitiveLayoutOffSelector: Int

var kCaseSensitiveLayoutOnSelector: Int

var kCaseSensitiveLayoutType: Int

var kCaseSensitiveSpacingOffSelector: Int

var kCaseSensitiveSpacingOnSelector: Int

var kCharacterAlternativesType: Int

var kCharacterShapeType: Int

var kCircleAnnotationSelector: Int

var kCommonLigaturesOffSelector: Int

var kCommonLigaturesOnSelector: Int

var kCompatibilityCompositionOffSelector: Int

var kCompatibilityCompositionOnSelector: Int

var kContextualAlternatesOffSelector: Int

var kContextualAlternatesOnSelector: Int

var kContextualAlternatesType: Int

var kContextualLigaturesOffSelector: Int

var kContextualLigaturesOnSelector: Int

var kContextualSwashAlternatesOffSelector: Int

var kContextualSwashAlternatesOnSelector: Int

var kCursiveConnectionType: Int

var kCursiveSelector: Int

var kDecomposeDiacriticsSelector: Int

var kDecorativeBordersSelector: Int

var kDefaultCJKRomanSelector: Int

var kDefaultLowerCaseSelector: Int

var kDefaultUpperCaseSelector: Int

var kDesignComplexityType: Int

var kDesignLevel1Selector: Int

var kDesignLevel2Selector: Int

var kDesignLevel3Selector: Int

var kDesignLevel4Selector: Int

var kDesignLevel5Selector: Int

var kDiacriticsType: Int

var kDiagonalFractionsSelector: Int

var kDiamondAnnotationSelector: Int

var kDingbatsSelector: Int

var kDiphthongLigaturesOffSelector: Int

var kDiphthongLigaturesOnSelector: Int

var kDisplayTextSelector: Int

var kEngravedTextSelector: Int

var kExpertCharactersSelector: Int

var kExponentsOffSelector: Int

var kExponentsOnSelector: Int

var kFleuronsSelector: Int

var kFontAlbanianLanguage: Int

var kFontAmharicLanguage: Int

var kFontAmharicScript: Int

var kFontArabicLanguage: Int

var kFontArabicScript: Int

var kFontArmenianLanguage: Int

var kFontArmenianScript: Int

var kFontAssameseLanguage: Int

var kFontAymaraLanguage: Int

var kFontAzerbaijanArLanguage: Int

var kFontAzerbaijaniLanguage: Int

var kFontBasqueLanguage: Int

var kFontBengaliLanguage: Int

var kFontBengaliScript: Int

var kFontBulgarianLanguage: Int

var kFontBurmeseLanguage: Int

var kFontBurmeseScript: Int

var kFontByelorussianLanguage: Int

var kFontCatalanLanguage: Int

var kFontChewaLanguage: Int

var kFontChineseScript: Int

var kFontCopyrightName: Int

var kFontCroatianLanguage: Int

var kFontCustom16BitScript: Int

var kFontCustom816BitScript: Int

var kFontCustom8BitScript: Int

var kFontCustomPlatform: Int

var kFontCyrillicScript: Int

var kFontCzechLanguage: Int

var kFontDanishLanguage: Int

var kFontDescriptionName: Int

var kFontDesignerName: Int

var kFontDesignerURLName: Int

var kFontDevanagariScript: Int

var kFontDutchLanguage: Int

var kFontDzongkhaLanguage: Int

var kFontEastEuropeanRomanScript: Int

var kFontEnglishLanguage: Int

var kFontEsperantoLanguage: Int

var kFontEstonianLanguage: Int

var kFontEthiopicScript: Int

var kFontExtendedArabicScript: Int

var kFontFaeroeseLanguage: Int

var kFontFamilyName: Int

var kFontFarsiLanguage: Int

var kFontFinnishLanguage: Int

var kFontFlemishLanguage: Int

var kFontFrenchLanguage: Int

var kFontFullName: Int

var kFontGallaLanguage: Int

var kFontGeezScript: Int

var kFontGeorgianLanguage: Int

var kFontGeorgianScript: Int

var kFontGermanLanguage: Int

var kFontGreekLanguage: Int

var kFontGreekScript: Int

var kFontGuaraniLanguage: Int

var kFontGujaratiLanguage: Int

var kFontGujaratiScript: Int

var kFontGurmukhiScript: Int

var kFontHebrewLanguage: Int

var kFontHebrewScript: Int

var kFontHindiLanguage: Int

var kFontHungarianLanguage: Int

var kFontISO10646_1993Semantics: Int

var kFontIcelandicLanguage: Int

var kFontIndonesianLanguage: Int

var kFontIrishLanguage: Int

var kFontItalianLanguage: Int

var kFontJapaneseLanguage: Int

var kFontJapaneseScript: Int

var kFontJavaneseRomLanguage: Int

var kFontKannadaLanguage: Int

var kFontKannadaScript: Int

var kFontKashmiriLanguage: Int

var kFontKazakhLanguage: Int

var kFontKhmerLanguage: Int

var kFontKhmerScript: Int

var kFontKirghizLanguage: Int

var kFontKoreanLanguage: Int

var kFontKoreanScript: Int

var kFontKurdishLanguage: Int

var kFontLaoLanguage: Int

var kFontLaotianScript: Int

var kFontLappishLanguage: Int

var kFontLastReservedName: Int

var kFontLatinLanguage: Int

var kFontLatvianLanguage: Int

var kFontLettishLanguage: Int

var kFontLicenseDescriptionName: Int

var kFontLicenseInfoURLName: Int

var kFontLithuanianLanguage: Int

var kFontMacCompatibleFullName: Int

var kFontMacedonianLanguage: Int

var kFontMacintoshPlatform: Int

var kFontMalagasyLanguage: Int

var kFontMalayArabicLanguage: Int

var kFontMalayRomanLanguage: Int

var kFontMalayalamLanguage: Int

var kFontMalayalamScript: Int

var kFontMalteseLanguage: Int

var kFontManufacturerName: Int

var kFontMarathiLanguage: Int

var kFontMicrosoftPlatform: Int

var kFontMicrosoftStandardScript: Int

var kFontMicrosoftSymbolScript: Int

var kFontMicrosoftUCS4Script: Int

var kFontMoldavianLanguage: Int

var kFontMongolianCyrLanguage: Int

var kFontMongolianLanguage: Int

var kFontMongolianScript: Int

var kFontNepaliLanguage: Int

var kFontNoLanguageCode: UInt32

var kFontNoNameCode: UInt32

var kFontNoPlatformCode: UInt32

var kFontNoScriptCode: UInt32

var kFontNorwegianLanguage: Int

var kFontOriyaLanguage: Int

var kFontOriyaScript: Int

var kFontOromoLanguage: Int

var kFontPashtoLanguage: Int

var kFontPersianLanguage: Int

var kFontPolishLanguage: Int

var kFontPortugueseLanguage: Int

var kFontPostScriptCIDName: Int

var kFontPostscriptName: Int

var kFontPreferredFamilyName: Int

var kFontPreferredSubfamilyName: Int

var kFontPunjabiLanguage: Int

var kFontQuechuaLanguage: Int

var kFontRSymbolScript: Int

var kFontReservedPlatform: Int

var kFontRomanScript: Int

var kFontRomanianLanguage: Int

var kFontRuandaLanguage: Int

var kFontRundiLanguage: Int

var kFontRussian: Int

var kFontRussianLanguage: Int

var kFontSaamiskLanguage: Int

var kFontSampleTextName: Int

var kFontSanskritLanguage: Int

var kFontSerbianLanguage: Int

var kFontSimpChineseLanguage: Int

var kFontSimpleChineseScript: Int

var kFontSindhiLanguage: Int

var kFontSindhiScript: Int

var kFontSinhaleseLanguage: Int

var kFontSinhaleseScript: Int

var kFontSlavicScript: Int

var kFontSlovakLanguage: Int

var kFontSlovenianLanguage: Int

var kFontSomaliLanguage: Int

var kFontSpanishLanguage: Int

var kFontStyleName: Int

var kFontSundaneseRomLanguage: Int

var kFontSwahiliLanguage: Int

var kFontSwedishLanguage: Int

var kFontTagalogLanguage: Int

var kFontTajikiLanguage: Int

var kFontTamilLanguage: Int

var kFontTamilScript: Int

var kFontTatarLanguage: Int

var kFontTeluguLanguage: Int

var kFontTeluguScript: Int

var kFontThaiLanguage: Int

var kFontThaiScript: Int

var kFontTibetanLanguage: Int

var kFontTibetanScript: Int

var kFontTigrinyaLanguage: Int

var kFontTradChineseLanguage: Int

var kFontTrademarkName: Int

var kFontTraditionalChineseScript: Int

var kFontTurkishLanguage: Int

var kFontTurkmenLanguage: Int

var kFontUighurLanguage: Int

var kFontUkrainianLanguage: Int

var kFontUnicodeDefaultSemantics: Int

var kFontUnicodePlatform: Int

var kFontUnicodeV1_1Semantics: Int

var kFontUnicodeV2_0BMPOnlySemantics: Int

var kFontUnicodeV2_0FullCoverageSemantics: Int

var kFontUnicodeV4_0VariationSequenceSemantics: Int

var kFontUnicode_FullRepertoire: Int

var kFontUninterpretedScript: Int

var kFontUniqueName: Int

var kFontUrduLanguage: Int

var kFontUzbekLanguage: Int

var kFontVendorURLName: Int

var kFontVersionName: Int

var kFontVietnameseLanguage: Int

var kFontVietnameseScript: Int

var kFontWelshLanguage: Int

var kFontYiddishLanguage: Int

var kFormInterrobangOffSelector: Int

var kFormInterrobangOnSelector: Int

var kFractionsType: Int

var kFullWidthCJKRomanSelector: Int

var kFullWidthIdeographsSelector: Int

var kFullWidthKanaSelector: Int

var kHalfWidthCJKRomanSelector: Int

var kHalfWidthIdeographsSelector: Int

var kHalfWidthTextSelector: Int

var kHanjaToHangulAltOneSelector: Int

var kHanjaToHangulAltThreeSelector: Int

var kHanjaToHangulAltTwoSelector: Int

var kHanjaToHangulSelector: Int

var kHideDiacriticsSelector: Int

var kHiraganaToKatakanaSelector: Int

var kHistoricalLigaturesOffSelector: Int

var kHistoricalLigaturesOnSelector: Int

var kHojoCharactersSelector: Int

var kHyphenToEnDashOffSelector: Int

var kHyphenToEnDashOnSelector: Int

var kHyphenToMinusOffSelector: Int

var kHyphenToMinusOnSelector: Int

var kHyphensToEmDashOffSelector: Int

var kHyphensToEmDashOnSelector: Int

var kIdeographicAltFiveSelector: Int

var kIdeographicAltFourSelector: Int

var kIdeographicAltOneSelector: Int

var kIdeographicAltThreeSelector: Int

var kIdeographicAltTwoSelector: Int

var kIdeographicAlternativesType: Int

var kIdeographicSpacingType: Int

var kIlluminatedCapsSelector: Int

var kInequalityLigaturesOffSelector: Int

var kInequalityLigaturesOnSelector: Int

var kInferiorsSelector: Int

var kInitialCapsAndSmallCapsSelector: Int

var kInitialCapsSelector: Int

var kInternationalSymbolsSelector: Int

var kInvertedBoxAnnotationSelector: Int

var kInvertedCircleAnnotationSelector: Int

var kInvertedRoundedBoxAnnotationSelector: Int

var kItalicCJKRomanType: Int

var kJIS1978CharactersSelector: Int

var kJIS1983CharactersSelector: Int

var kJIS1990CharactersSelector: Int

var kJIS2004CharactersSelector: Int

var kJUSTCurrentVersion: Int

var kJUSTKashidaPriority: Int

var kJUSTLetterPriority: Int

var kJUSTNullPriority: Int

var kJUSTOverrideLimits: Int

var kJUSTOverridePriority: Int

var kJUSTOverrideUnlimited: Int

var kJUSTPriorityCount: Int

var kJUSTPriorityMask: Int

var kJUSTSpacePriority: Int

var kJUSTStandardFormat: Int

var kJUSTTag: Int

var kJUSTUnlimited: Int

var kJUSTnoGlyphcode: Int

var kJUSTpcConditionalAddAction: Int

var kJUSTpcDecompositionAction: Int

var kJUSTpcDuctilityAction: Int

var kJUSTpcGlyphRepeatAddAction: Int

var kJUSTpcGlyphStretchAction: Int

var kJUSTpcUnconditionalAddAction: Int

var kKERNCrossStream: Int

var kKERNCrossStreamResetNote: Int

var kKERNCurrentVersion: Int

var kKERNFormatMask: Int

var kKERNIndexArray: Int

var kKERNLineEndKerning: Int

var kKERNLineStart: Int

var kKERNNoCrossKerning: Int

var kKERNNoStakeNote: Int

var kKERNNotApplied: Int

var kKERNNotesRequested: Int

var kKERNOrderedList: Int

var kKERNResetCrossStream: Int

var kKERNSimpleArray: Int

var kKERNStateTable: Int

var kKERNTag: Int

var kKERNUnusedBits: Int

var kKERNVariation: Int

var kKERNVertical: Int

var kKERXActionOffsetMask: UInt32

var kKERXActionTypeAnchorPoints: UInt32

var kKERXActionTypeControlPoints: UInt32

var kKERXActionTypeCoordinates: UInt32

var kKERXActionTypeMask: UInt32

var kKERXControlPoint: Int

var kKERXCrossStream: Int

var kKERXCrossStreamResetNote: Int

var kKERXCurrentVersion: Int

var kKERXFormatMask: Int

var kKERXIndexArray: Int

var kKERXLineEndKerning: Int

var kKERXLineStart: Int

var kKERXNoCrossKerning: Int

var kKERXNoStakeNote: Int

var kKERXNotApplied: Int

var kKERXNotesRequested: Int

var kKERXOrderedList: Int

var kKERXResetCrossStream: Int

var kKERXSimpleArray: Int

var kKERXStateTable: Int

var kKERXTag: Int

var kKERXUnusedBits: Int

var kKERXUnusedFlags: UInt32

var kKERXVariation: Int

var kKERXVertical: Int

var kKanaSpacingType: Int

var kKanaToRomanizationSelector: Int

var kKatakanaToHiraganaSelector: Int

var kLCARCtlPointFormat: Int

var kLCARCurrentVersion: Int

var kLCARLinearFormat: Int

var kLCARTag: Int

var kLastFeatureType: Int

var kLetterCaseType: Int

var kLigaturesType: Int

var kLineFinalSwashesOffSelector: Int

var kLineFinalSwashesOnSelector: Int

var kLineInitialSwashesOffSelector: Int

var kLineInitialSwashesOnSelector: Int

var kLinguisticRearrangementOffSelector: Int

var kLinguisticRearrangementOnSelector: Int

var kLinguisticRearrangementType: Int

var kLogosOffSelector: Int

var kLogosOnSelector: Int

var kLowerCaseNumbersSelector: Int

var kLowerCasePetiteCapsSelector: Int

var kLowerCaseSmallCapsSelector: Int

var kLowerCaseType: Int

var kMORTContextualType: Int

var kMORTCoverDescending: Int

var kMORTCoverIgnoreVertical: Int

var kMORTCoverTypeMask: Int

var kMORTCoverVertical: Int

var kMORTCurrInsertBefore: Int

var kMORTCurrInsertCountMask: Int

var kMORTCurrInsertCountShift: Int

var kMORTCurrInsertKashidaLike: Int

var kMORTCurrJustTableCountMask: Int

var kMORTCurrJustTableCountShift: Int

var kMORTCurrentVersion: Int

var kMORTDoInsertionsBefore: Int

var kMORTInsertionType: Int

var kMORTInsertionsCountMask: Int

var kMORTIsSplitVowelPiece: Int

var kMORTLigFormOffsetMask: Int

var kMORTLigFormOffsetShift: Int

var kMORTLigLastAction: Int

var kMORTLigStoreLigature: Int

var kMORTLigatureType: Int

var kMORTMarkInsertBefore: Int

var kMORTMarkInsertCountMask: Int

var kMORTMarkInsertCountShift: Int

var kMORTMarkInsertKashidaLike: Int

var kMORTMarkJustTableCountMask: Int

var kMORTMarkJustTableCountShift: Int

var kMORTRearrangementType: Int

var kMORTSwashType: Int

var kMORTTag: Int

var kMORTraCDx: Int

var kMORTraCDxA: Int

var kMORTraCDxAB: Int

var kMORTraCDxBA: Int

var kMORTraDCx: Int

var kMORTraDCxA: Int

var kMORTraDCxAB: Int

var kMORTraDCxBA: Int

var kMORTraDx: Int

var kMORTraDxA: Int

var kMORTraDxAB: Int

var kMORTraDxBA: Int

var kMORTraNoAction: Int

var kMORTraxA: Int

var kMORTraxAB: Int

var kMORTraxBA: Int

var kMORXCoverDescending: Int

var kMORXCoverIgnoreVertical: Int

var kMORXCoverTypeMask: Int

var kMORXCoverVertical: Int

var kMORXCurrentVersion: Int

var kMORXTag: Int

var kMathSymbolsSelector: Int

var kMathematicalExtrasType: Int

var kMathematicalGreekOffSelector: Int

var kMathematicalGreekOnSelector: Int

var kMonospacedNumbersSelector: Int

var kMonospacedTextSelector: Int

var kNLCCharactersSelector: Int

var kNoAlternatesSelector: Int

var kNoAnnotationSelector: Int

var kNoCJKItalicRomanSelector: Int

var kNoCJKSymbolAlternativesSelector: Int

var kNoFractionsSelector: Int

var kNoIdeographicAlternativesSelector: Int

var kNoOrnamentsSelector: Int

var kNoRubyKanaSelector: Int

var kNoStyleOptionsSelector: Int

var kNoStylisticAlternatesSelector: Int

var kNoTransliterationSelector: Int

var kNonFinalSwashesOffSelector: Int

var kNonFinalSwashesOnSelector: Int

var kNormalPositionSelector: Int

var kNumberCaseType: Int

var kNumberSpacingType: Int

var kOPBDControlPointFormat: Int

var kOPBDCurrentVersion: Int

var kOPBDDistanceFormat: Int

var kOPBDTag: Int

var kOrdinalsSelector: Int

var kOrnamentSetsType: Int

var kOverlappingCharactersType: Int

var kPROPALDirectionClass: Int

var kPROPANDirectionClass: Int

var kPROPBNDirectionClass: Int

var kPROPCSDirectionClass: Int

var kPROPCanHangLTMask: Int

var kPROPCanHangRBMask: Int

var kPROPCurrentVersion: Int

var kPROPDirectionMask: Int

var kPROPENDirectionClass: Int

var kPROPESDirectionClass: Int

var kPROPETDirectionClass: Int

var kPROPIsFloaterMask: Int

var kPROPLDirectionClass: Int

var kPROPLREDirectionClass: Int

var kPROPLRODirectionClass: Int

var kPROPNSMDirectionClass: Int

var kPROPNumDirectionClasses: Int

var kPROPONDirectionClass: Int

var kPROPPDFDirectionClass: Int

var kPROPPSDirectionClass: Int

var kPROPPairOffsetMask: Int

var kPROPPairOffsetShift: Int

var kPROPPairOffsetSign: Int

var kPROPRDirectionClass: Int

var kPROPRLEDirectionClass: Int

var kPROPRLODirectionClass: Int

var kPROPRightConnectMask: Int

var kPROPSDirectionClass: Int

var kPROPSENDirectionClass: Int

var kPROPTag: Int

var kPROPUseRLPairMask: Int

var kPROPWSDirectionClass: Int

var kPROPZeroReserved: Int

var kParenthesisAnnotationSelector: Int

var kPartiallyConnectedSelector: Int

var kPeriodAnnotationSelector: Int

var kPeriodsToEllipsisOffSelector: Int

var kPeriodsToEllipsisOnSelector: Int

var kPiCharactersSelector: Int

var kPreventOverlapOffSelector: Int

var kPreventOverlapOnSelector: Int

var kProportionalCJKRomanSelector: Int

var kProportionalIdeographsSelector: Int

var kProportionalKanaSelector: Int

var kProportionalNumbersSelector: Int

var kProportionalTextSelector: Int

var kQuarterWidthNumbersSelector: Int

var kQuarterWidthTextSelector: Int

var kRareLigaturesOffSelector: Int

var kRareLigaturesOnSelector: Int

var kRebusPicturesOffSelector: Int

var kRebusPicturesOnSelector: Int

var kRequiredLigaturesOffSelector: Int

var kRequiredLigaturesOnSelector: Int

var kRomanNumeralAnnotationSelector: Int

var kRomanizationToHiraganaSelector: Int

var kRomanizationToKatakanaSelector: Int

var kRoundedBoxAnnotationSelector: Int

var kRubyKanaOffSelector: Int

var kRubyKanaOnSelector: Int

var kRubyKanaSelector: Int

var kRubyKanaType: Int

var kSFNTLookupSegmentArray: Int

var kSFNTLookupSegmentSingle: Int

var kSFNTLookupSimpleArray: Int

var kSFNTLookupSingleTable: Int

var kSFNTLookupTrimmedArray: Int

var kSFNTLookupVector: Int

var kSTClassDeletedGlyph: Int

var kSTClassEndOfLine: Int

var kSTClassEndOfText: Int

var kSTClassOutOfBounds: Int

var kSTLigActionMask: Int

var kSTMarkEnd: Int

var kSTNoAdvance: Int

var kSTRearrVerbMask: Int

var kSTSetMark: Int

var kSTXHasLigAction: Int

var kScientificInferiorsSelector: Int

var kShowDiacriticsSelector: Int

var kSimplifiedCharactersSelector: Int

var kSlashToDivideOffSelector: Int

var kSlashToDivideOnSelector: Int

var kSlashedZeroOffSelector: Int

var kSlashedZeroOnSelector: Int

var kSmallCapsSelector: Int

var kSmartQuotesOffSelector: Int

var kSmartQuotesOnSelector: Int

var kSmartSwashType: Int

var kSquaredLigaturesOffSelector: Int

var kSquaredLigaturesOnSelector: Int

var kStyleOptionsType: Int

var kStylisticAltEightOffSelector: Int

var kStylisticAltEightOnSelector: Int

var kStylisticAltEighteenOffSelector: Int

var kStylisticAltEighteenOnSelector: Int

var kStylisticAltElevenOffSelector: Int

var kStylisticAltElevenOnSelector: Int

var kStylisticAltFifteenOffSelector: Int

var kStylisticAltFifteenOnSelector: Int

var kStylisticAltFiveOffSelector: Int

var kStylisticAltFiveOnSelector: Int

var kStylisticAltFourOffSelector: Int

var kStylisticAltFourOnSelector: Int

var kStylisticAltFourteenOffSelector: Int

var kStylisticAltFourteenOnSelector: Int

var kStylisticAltNineOffSelector: Int

var kStylisticAltNineOnSelector: Int

var kStylisticAltNineteenOffSelector: Int

var kStylisticAltNineteenOnSelector: Int

var kStylisticAltOneOffSelector: Int

var kStylisticAltOneOnSelector: Int

var kStylisticAltSevenOffSelector: Int

var kStylisticAltSevenOnSelector: Int

var kStylisticAltSeventeenOffSelector: Int

var kStylisticAltSeventeenOnSelector: Int

var kStylisticAltSixOffSelector: Int

var kStylisticAltSixOnSelector: Int

var kStylisticAltSixteenOffSelector: Int

var kStylisticAltSixteenOnSelector: Int

var kStylisticAltTenOffSelector: Int

var kStylisticAltTenOnSelector: Int

var kStylisticAltThirteenOffSelector: Int

var kStylisticAltThirteenOnSelector: Int

var kStylisticAltThreeOffSelector: Int

var kStylisticAltThreeOnSelector: Int

var kStylisticAltTwelveOffSelector: Int

var kStylisticAltTwelveOnSelector: Int

var kStylisticAltTwentyOffSelector: Int

var kStylisticAltTwentyOnSelector: Int

var kStylisticAltTwoOffSelector: Int

var kStylisticAltTwoOnSelector: Int

var kStylisticAlternativesType: Int

var kSubstituteVerticalFormsOffSelector: Int

var kSubstituteVerticalFormsOnSelector: Int

var kSuperiorsSelector: Int

var kSwashAlternatesOffSelector: Int

var kSwashAlternatesOnSelector: Int

var kSymbolLigaturesOffSelector: Int

var kSymbolLigaturesOnSelector: Int

var kTRAKCurrentVersion: Int

var kTRAKTag: Int

var kTRAKUniformFormat: Int

var kTallCapsSelector: Int

var kTextSpacingType: Int

var kThirdWidthNumbersSelector: Int

var kThirdWidthTextSelector: Int

var kTitlingCapsSelector: Int

var kTraditionalAltFiveSelector: Int

var kTraditionalAltFourSelector: Int

var kTraditionalAltOneSelector: Int

var kTraditionalAltThreeSelector: Int

var kTraditionalAltTwoSelector: Int

var kTraditionalCharactersSelector: Int

var kTraditionalNamesCharactersSelector: Int

var kTranscodingCompositionOffSelector: Int

var kTranscodingCompositionOnSelector: Int

var kTransliterationType: Int

var kTypographicExtrasType: Int

var kUnconnectedSelector: Int

var kUnicodeDecompositionType: Int

var kUpperAndLowerCaseSelector: Int

var kUpperCaseNumbersSelector: Int

var kUpperCasePetiteCapsSelector: Int

var kUpperCaseSmallCapsSelector: Int

var kUpperCaseType: Int

var kVerticalFractionsSelector: Int

var kVerticalPositionType: Int

var kVerticalSubstitutionType: Int

var kWordFinalSwashesOffSelector: Int

var kWordFinalSwashesOnSelector: Int

var kWordInitialSwashesOffSelector: Int

var kWordInitialSwashesOnSelector: Int

var nameFontTableTag: Int

var nonGlyphID: Int

var os2FontTableTag: Int

var sizeof_sfntCMapEncoding: Int

var sizeof_sfntCMapExtendedSubHeader: Int

var sizeof_sfntCMapHeader: Int

var sizeof_sfntCMapSubHeader: Int

var sizeof_sfntDescriptorHeader: Int

var sizeof_sfntDirectory: Int

var sizeof_sfntInstance: Int

var sizeof_sfntNameHeader: Int

var sizeof_sfntNameRecord: Int

var sizeof_sfntVariationAxis: Int

var sizeof_sfntVariationHeader: Int

var variationFontTableTag: Int

## See Also

### Reference

Styling Attributed Strings

Attributes to which Core Text responds when placed in a `CFAttributedString` object.

Core Text Structures

Core Text Enumerations

Core Text Constants

Core Text Functions

Core Text Data Types

