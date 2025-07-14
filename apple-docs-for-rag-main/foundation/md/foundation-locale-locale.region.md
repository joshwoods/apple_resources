

- Foundation
- Locale
-  Locale.Region 

Structure

# Locale.Region

A type that represents a geographic region, for use in specifying a locale or language.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Region
```

## Topics

### Creating a region

init(String)

Creates a region from a BCP 47 identifier.

### Examining region properties

var identifier: String

The BCP 47 identifier of the region.

var containingRegion: Locale.Region?

The region that contains this region, if any.

var continent: Locale.Region?

The continent that contains this region, if any.

var isISORegion: Bool

A Boolean value that indicates whether the region is an ISO-defined region.

var subRegions: [Locale.Region]

An array of all the sub-regions of the region.

### Using special-purpose regions

static let unknown: Locale.Region

A pre-defined unknown or invalid region.

### Getting a list of regions

static var isoRegions: [Locale.Region]

An array of regions defined by ISO.

### Type Properties

static var ålandIslands: Locale.Region

static var afghanistan: Locale.Region

static var albania: Locale.Region

static var algeria: Locale.Region

static var americanSamoa: Locale.Region

static var andorra: Locale.Region

static var angola: Locale.Region

static var anguilla: Locale.Region

static var antarctica: Locale.Region

static var antiguaBarbuda: Locale.Region

static var argentina: Locale.Region

static var armenia: Locale.Region

static var aruba: Locale.Region

static var ascensionIsland: Locale.Region

static var australia: Locale.Region

static var austria: Locale.Region

static var azerbaijan: Locale.Region

static var bahamas: Locale.Region

static var bahrain: Locale.Region

static var bangladesh: Locale.Region

static var barbados: Locale.Region

static var belarus: Locale.Region

static var belgium: Locale.Region

static var belize: Locale.Region

static var benin: Locale.Region

static var bermuda: Locale.Region

static var bhutan: Locale.Region

static var bolivia: Locale.Region

static var bosniaHerzegovina: Locale.Region

static var botswana: Locale.Region

static var bouvetIsland: Locale.Region

static var brazil: Locale.Region

static var britishVirginIslands: Locale.Region

static var brunei: Locale.Region

static var bulgaria: Locale.Region

static var burkinaFaso: Locale.Region

static var burundi: Locale.Region

static var côteDIvoire: Locale.Region

static var cambodia: Locale.Region

static var cameroon: Locale.Region

static var canada: Locale.Region

static var canaryIslands: Locale.Region

static var capeVerde: Locale.Region

static var caribbeanNetherlands: Locale.Region

static var caymanIslands: Locale.Region

static var centralAfricanRepublic: Locale.Region

static var ceutaMelilla: Locale.Region

static var chad: Locale.Region

static var chagosArchipelago: Locale.Region

static var chile: Locale.Region

static var chinaMainland: Locale.Region

static var christmasIsland: Locale.Region

static var clippertonIsland: Locale.Region

static var cocosIslands: Locale.Region

static var colombia: Locale.Region

static var comoros: Locale.Region

static var congoBrazzaville: Locale.Region

static var congoKinshasa: Locale.Region

static var cookIslands: Locale.Region

static var costaRica: Locale.Region

static var croatia: Locale.Region

static var cuba: Locale.Region

static var curaçao: Locale.Region

static var cyprus: Locale.Region

static var czechia: Locale.Region

static var denmark: Locale.Region

static var diegoGarcia: Locale.Region

static var djibouti: Locale.Region

static var dominica: Locale.Region

static var dominicanRepublic: Locale.Region

static var ecuador: Locale.Region

static var egypt: Locale.Region

static var elSalvador: Locale.Region

static var equatorialGuinea: Locale.Region

static var eritrea: Locale.Region

static var estonia: Locale.Region

static var eswatini: Locale.Region

static var ethiopia: Locale.Region

static var falklandIslands: Locale.Region

static var faroeIslands: Locale.Region

static var fiji: Locale.Region

static var finland: Locale.Region

static var france: Locale.Region

static var frenchGuiana: Locale.Region

static var frenchPolynesia: Locale.Region

static var frenchSouthernTerritories: Locale.Region

static var gabon: Locale.Region

static var gambia: Locale.Region

static var georgia: Locale.Region

static var germany: Locale.Region

static var ghana: Locale.Region

static var gibraltar: Locale.Region

static var greece: Locale.Region

static var greenland: Locale.Region

static var grenada: Locale.Region

static var guadeloupe: Locale.Region

static var guam: Locale.Region

static var guatemala: Locale.Region

static var guernsey: Locale.Region

static var guinea: Locale.Region

static var guineaBissau: Locale.Region

static var guyana: Locale.Region

static var haiti: Locale.Region

static var heardMcdonaldIslands: Locale.Region

static var honduras: Locale.Region

static var hongKong: Locale.Region

static var hungary: Locale.Region

static var iceland: Locale.Region

static var india: Locale.Region

static var indonesia: Locale.Region

static var iran: Locale.Region

static var iraq: Locale.Region

static var ireland: Locale.Region

static var isleOfMan: Locale.Region

static var israel: Locale.Region

static var italy: Locale.Region

static var jamaica: Locale.Region

static var japan: Locale.Region

static var jersey: Locale.Region

static var jordan: Locale.Region

static var kazakhstan: Locale.Region

static var kenya: Locale.Region

static var kiribati: Locale.Region

static var kosovo: Locale.Region

static var kuwait: Locale.Region

static var kyrgyzstan: Locale.Region

static var laos: Locale.Region

static var latinAmerica: Locale.Region

static var latvia: Locale.Region

static var lebanon: Locale.Region

static var lesotho: Locale.Region

static var liberia: Locale.Region

static var libya: Locale.Region

static var liechtenstein: Locale.Region

static var lithuania: Locale.Region

static var luxembourg: Locale.Region

static var macao: Locale.Region

static var madagascar: Locale.Region

static var malawi: Locale.Region

static var malaysia: Locale.Region

static var maldives: Locale.Region

static var mali: Locale.Region

static var malta: Locale.Region

static var marshallIslands: Locale.Region

static var martinique: Locale.Region

static var mauritania: Locale.Region

static var mauritius: Locale.Region

static var mayotte: Locale.Region

static var mexico: Locale.Region

static var micronesia: Locale.Region

static var moldova: Locale.Region

static var monaco: Locale.Region

static var mongolia: Locale.Region

static var montenegro: Locale.Region

static var montserrat: Locale.Region

static var morocco: Locale.Region

static var mozambique: Locale.Region

static var myanmar: Locale.Region

static var namibia: Locale.Region

static var nauru: Locale.Region

static var nepal: Locale.Region

static var netherlands: Locale.Region

static var newCaledonia: Locale.Region

static var newZealand: Locale.Region

static var nicaragua: Locale.Region

static var niger: Locale.Region

static var nigeria: Locale.Region

static var niue: Locale.Region

static var norfolkIsland: Locale.Region

static var northMacedonia: Locale.Region

static var northernMarianaIslands: Locale.Region

static var norway: Locale.Region

static var oman: Locale.Region

static var pakistan: Locale.Region

static var palau: Locale.Region

static var palestinianTerritories: Locale.Region

static var panama: Locale.Region

static var papuaNewGuinea: Locale.Region

static var paraguay: Locale.Region

static var peru: Locale.Region

static var philippines: Locale.Region

static var pitcairnIslands: Locale.Region

static var poland: Locale.Region

static var portugal: Locale.Region

static var puertoRico: Locale.Region

static var qatar: Locale.Region

static var réunion: Locale.Region

static var romania: Locale.Region

static var russia: Locale.Region

static var rwanda: Locale.Region

static var sãoToméPríncipe: Locale.Region

static var saintBarthélemy: Locale.Region

static var saintHelena: Locale.Region

static var saintKittsNevis: Locale.Region

static var saintLucia: Locale.Region

static var saintMartin: Locale.Region

static var saintPierreMiquelon: Locale.Region

static var saintVincentGrenadines: Locale.Region

static var samoa: Locale.Region

static var sanMarino: Locale.Region

static var saudiArabia: Locale.Region

static var senegal: Locale.Region

static var serbia: Locale.Region

static var seychelles: Locale.Region

static var sierraLeone: Locale.Region

static var singapore: Locale.Region

static var sintMaarten: Locale.Region

static var slovakia: Locale.Region

static var slovenia: Locale.Region

static var solomonIslands: Locale.Region

static var somalia: Locale.Region

static var southAfrica: Locale.Region

static var southGeorgiaSouthSandwichIslands: Locale.Region

static var southKorea: Locale.Region

static var southSudan: Locale.Region

static var spain: Locale.Region

static var sriLanka: Locale.Region

static var suriname: Locale.Region

static var svalbardJanMayen: Locale.Region

static var sweden: Locale.Region

static var switzerland: Locale.Region

static var taiwan: Locale.Region

static var tajikistan: Locale.Region

static var tanzania: Locale.Region

static var thailand: Locale.Region

static var timorLeste: Locale.Region

static var togo: Locale.Region

static var tokelau: Locale.Region

static var tonga: Locale.Region

static var trinidadTobago: Locale.Region

static var tristanDaCunha: Locale.Region

static var tunisia: Locale.Region

static var turkey: Locale.Region

static var turkmenistan: Locale.Region

static var turksCaicosIslands: Locale.Region

static var tuvalu: Locale.Region

static var uganda: Locale.Region

static var ukraine: Locale.Region

static var unitedArabEmirates: Locale.Region

static var unitedKingdom: Locale.Region

static var unitedStates: Locale.Region

static var unitedStatesOutlyingIslands: Locale.Region

static var unitedStatesVirginIslands: Locale.Region

static var uruguay: Locale.Region

static var uzbekistan: Locale.Region

static var vanuatu: Locale.Region

static var vaticanCity: Locale.Region

static var venezuela: Locale.Region

static var vietnam: Locale.Region

static var wallisFutuna: Locale.Region

static var westernSahara: Locale.Region

static var world: Locale.Region

static var yemen: Locale.Region

static var zambia: Locale.Region

static var zimbabwe: Locale.Region

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Decodable
- Encodable
- Equatable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Hashable
- Sendable

## See Also

### Getting region components

var region: Locale.Region?

The region used by the locale.

var subdivision: Locale.Subdivision?

The optional subdivision of the region used by this locale.

struct Subdivision

A type that represents a subdivision of a region, such as a state in the US or a province in Canada.

var variant: Locale.Variant?

An optional variant used by the locale.

struct Variant

A type that represents a locale’s languate variant.

