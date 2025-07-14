

- Contacts
-  CNLabeledValue 

Class

# CNLabeledValue

An immutable object that combines a contact property value with a label that describes that property.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class CNLabeledValue where ValueType : NSCopying, ValueType : NSSecureCoding
```

## Overview

Labels describe the context for a property. For example, the label for a phone number indicates whether it corresponds to the user’s home, work, or iPhone number.

`CNLabeledValue` objects are thread-safe, and you can access their properties from any thread of your app.

## Topics

### Creating a labeled value

init(label: String?, value: ValueType)

Returns a new labeled value identifier.

### Getting the label and value

var label: String?

The label for a contact property value.

var value: ValueType

A contact property value.

### Setting labels and values

func settingLabel(String?) -> Self

Returns a labeled value object with an existing value and identifier.

func settingLabel(String?, value: ValueType) -> Self

Returns a labeled value object with the specified label and value with the existing identifier.

func settingValue(ValueType) -> Self

Returns a new value for an existing label and identifier.

### Localizing the label and value

class func localizedString(forLabel: String) -> String

Returns a localized string for the specified label.

### Getting the unique identifier

var identifier: String

A unique identifier for the labeled value object.

### Getting common labels

let CNLabelHome: String

The label for identifying home information.

let CNLabelWork: String

The label for identifying work information.

let CNLabelSchool: String

The label for the contact’s school.

let CNLabelOther: String

The label for identifying other information.

let CNLabelEmailiCloud: String

The label for identifying the contact’s iCloud email information.

let CNLabelURLAddressHomePage: String

The label for identifying URL information.

let CNLabelDateAnniversary: String

The label for identifying the contact’s anniversary date.

### Getting phone number labels

let CNLabelPhoneNumberMain: String

The label for identifying the contact’s main phone number.

let CNLabelPhoneNumberiPhone: String

The label for identifying the contact’s iPhone number.

let CNLabelPhoneNumberAppleWatch: String

The label for identifying the contact’s Apple Watch phone number.

let CNLabelPhoneNumberMobile: String

The label for identifying the contact’s mobile phone number.

let CNLabelPhoneNumberPager: String

The label for identifying the contact’s pager number.

let CNLabelPhoneNumberWorkFax: String

The label for identifying the contact’s work fax number.

let CNLabelPhoneNumberHomeFax: String

The label for identifying the contact’s home fax number.

let CNLabelPhoneNumberOtherFax: String

The label for identifying another fax number.

### Getting immediate family relationship labels

let CNLabelContactRelationBrother: String

The label for the contact’s brother.

let CNLabelContactRelationChild: String

The label for the contact’s child.

let CNLabelContactRelationDaughter: String

The label for the contact’s daughter.

let CNLabelContactRelationElderBrother: String

The label for the contact’s elder brother.

let CNLabelContactRelationElderSibling: String

The label for the contact’s elder sibling.

let CNLabelContactRelationElderSister: String

The label for the contact’s elder sister.

let CNLabelContactRelationEldestBrother: String

The label for the contact’s eldest brother.

let CNLabelContactRelationEldestSister: String

The label for the contact’s eldest sister.

let CNLabelContactRelationFather: String

The label for the contact’s father.

let CNLabelContactRelationFemalePartner: String

The label for the contact’s female partner.

let CNLabelContactRelationHusband: String

The label for the contact’s husband.

let CNLabelContactRelationMalePartner: String

The label for the contact’s male partner.

let CNLabelContactRelationMother: String

The label for the contact’s mother.

let CNLabelContactRelationParent: String

The label for the contact’s parent.

let CNLabelContactRelationPartner: String

The label for the contact’s partner.

let CNLabelContactRelationSibling: String

The label for the contact’s sibling.

let CNLabelContactRelationSister: String

The label for the contact’s sister.

let CNLabelContactRelationSon: String

The label for the contact’s son.

let CNLabelContactRelationSpouse: String

The label for the contact’s spouse.

let CNLabelContactRelationStepbrother: String

The label for the contact’s stepbrother.

let CNLabelContactRelationStepchild: String

The label for the contact’s stepchild.

let CNLabelContactRelationStepdaughter: String

The label for the contact’s stepdaughter.

let CNLabelContactRelationStepfather: String

The label for the contact’s stepfather.

let CNLabelContactRelationStepmother: String

The label for the contact’s stepmother.

let CNLabelContactRelationStepparent: String

The label for the contact’s stepparent.

let CNLabelContactRelationStepsister: String

The label for the contact’s stepsister.

let CNLabelContactRelationStepson: String

The label for the contact’s stepson.

let CNLabelContactRelationWife: String

The label for the contact’s wife.

let CNLabelContactRelationYoungerBrother: String

The label for the contact’s younger brother.

let CNLabelContactRelationYoungerSibling: String

The label for the contact’s younger sibling.

let CNLabelContactRelationYoungerSister: String

The label for the contact’s younger sister.

let CNLabelContactRelationYoungestBrother: String

The label for the contact’s youngest brother.

let CNLabelContactRelationYoungestSister: String

The label for the contact’s youngest sister.

### Getting acquaintance relationship labels

let CNLabelContactRelationBoyfriend: String

The label for the contact’s boyfriend.

let CNLabelContactRelationColleague: String

The label for the contact’s colleague.

let CNLabelContactRelationFemaleFriend: String

The label for the contact’s female friend.

let CNLabelContactRelationFriend: String

The label for the contact’s friend.

let CNLabelContactRelationGirlfriend: String

The label for the contact’s girlfriend.

let CNLabelContactRelationGirlfriendOrBoyfriend: String

The label for the contact’s girlfriend or boyfriend.

let CNLabelContactRelationMaleFriend: String

The label for the contact’s male friend.

### Getting business relationship labels

let CNLabelContactRelationAssistant: String

The label for the contact’s assistant.

let CNLabelContactRelationManager: String

The label for the contact’s manager.

### Getting education relationship labels

let CNLabelContactRelationTeacher: String

The label for the contact’s teacher.

### Getting in-law relationship labels

let CNLabelContactRelationBrotherInLaw: String

The label for the contact’s brother-in-law.

let CNLabelContactRelationBrotherInLawElderSistersHusband: String

The label for the contact’s elder sister’s husband.

let CNLabelContactRelationBrotherInLawHusbandsBrother: String

The label for the contact’s husband’s brother.

let CNLabelContactRelationBrotherInLawHusbandsSistersHusband: String

The label for the contact’s husband’s sister’s husband.

let CNLabelContactRelationBrotherInLawSistersHusband: String

The label for the contact’s sister’s husband.

let CNLabelContactRelationBrotherInLawSpousesBrother: String

The label for the contact’s spouse’s brother.

let CNLabelContactRelationBrotherInLawWifesBrother: String

The label for the contact’s wife’s brother.

let CNLabelContactRelationBrotherInLawWifesSistersHusband: String

The label for the contact’s wife’s sister’s husband.

let CNLabelContactRelationBrotherInLawYoungerSistersHusband: String

The label for the contact’s younger sister’s husband.

let CNLabelContactRelationChildInLaw: String

The label for the contact’s child-in-law.

let CNLabelContactRelationCoBrotherInLaw: String

The label for the contact’s co-brother-in-law.

let CNLabelContactRelationCoFatherInLaw: String

The label for the contact’s co-father-in-law.

let CNLabelContactRelationCoMotherInLaw: String

The label for the contact’s co-mother-in-law.

let CNLabelContactRelationCoParentInLaw: String

The label for the contact’s co-parent-in-law.

let CNLabelContactRelationCoSiblingInLaw: String

The label for the contact’s co-sibling-in-law.

let CNLabelContactRelationCoSisterInLaw: String

The label for the contact’s co-sister-in-law.

let CNLabelContactRelationElderBrotherInLaw: String

The label for the contact’s elder brother-in-law.

let CNLabelContactRelationElderSiblingInLaw: String

The label for the contact’s elder sibling-in-law.

let CNLabelContactRelationElderSisterInLaw: String

The label for the contact’s elder sister-in-law.

let CNLabelContactRelationFatherInLaw: String

The label for the contact’s father-in-law.

let CNLabelContactRelationFatherInLawHusbandsFather: String

The label for the contact’s husband’s father.

let CNLabelContactRelationFatherInLawOrStepfather: String

The label for the contact’s father-in-law or stepfather.

let CNLabelContactRelationFatherInLawWifesFather: String

The label for the contact’s wife’s father.

let CNLabelContactRelationMotherInLaw: String

The label for the contact’s mother-in-law.

let CNLabelContactRelationMotherInLawHusbandsMother: String

The label for the contact’s husband’s mother.

let CNLabelContactRelationMotherInLawOrStepmother: String

The label for the contact’s mother-in-law or stepmother.

let CNLabelContactRelationMotherInLawWifesMother: String

The label for the contact’s wife’s mother.

let CNLabelContactRelationParentInLaw: String

The label for the contact’s parent-in-law.

let CNLabelContactRelationSiblingInLaw: String

The label for the contact’s sibling-in-law.

let CNLabelContactRelationSisterInLaw: String

The label for the contact’s sister-in-law.

let CNLabelContactRelationSisterInLawBrothersWife: String

The label for the contact’s brother’s wife.

let CNLabelContactRelationSisterInLawElderBrothersWife: String

The label for the contact’s elder brother’s wife.

let CNLabelContactRelationSisterInLawHusbandsBrothersWife: String

The label for the contact’s husband’s brother’s wife.

let CNLabelContactRelationSisterInLawHusbandsSister: String

The label for the contact’s husband’s sister.

let CNLabelContactRelationSisterInLawSpousesSister: String

The label for the contact’s spouse’s sister.

let CNLabelContactRelationSisterInLawWifesBrothersWife: String

The label for the contact’s wife’s brother’s wife.

let CNLabelContactRelationSisterInLawWifesSister: String

The label for the contact’s wife’s sister.

let CNLabelContactRelationSisterInLawYoungerBrothersWife: String

The label for the contact’s younger brother’s wife.

let CNLabelContactRelationYoungerBrotherInLaw: String

The label for the contact’s younger brother-in-law.

let CNLabelContactRelationYoungerSiblingInLaw: String

The label for the contact’s younger sibling-in-law.

let CNLabelContactRelationYoungerSisterInLaw: String

The label for the contact’s younger sister-in-law.

### Getting extended family relationship labels

let CNLabelContactRelationAunt: String

The label for the contact’s aunt.

let CNLabelContactRelationAuntFathersBrothersWife: String

The label for the contact’s father’s brother’s wife.

let CNLabelContactRelationAuntFathersElderBrothersWife: String

The label for the contact’s father’s elder brother’s wife.

let CNLabelContactRelationAuntFathersElderSister: String

The label for the contact’s father’s elder sister.

let CNLabelContactRelationAuntFathersSister: String

The label for the contact’s father’s sister.

let CNLabelContactRelationAuntFathersYoungerBrothersWife: String

The label for the contact’s father’s younger brother’s wife.

let CNLabelContactRelationAuntFathersYoungerSister: String

The label for the contact’s father’s younger sister.

let CNLabelContactRelationAuntMothersBrothersWife: String

The label for the contact’s mother’s brother’s wife.

let CNLabelContactRelationAuntMothersElderSister: String

The label for the contact’s mother’s elder sister.

let CNLabelContactRelationAuntMothersSister: String

The label for the contact’s mother’s sister.

let CNLabelContactRelationAuntMothersYoungerSister: String

The label for the contact’s mother’s younger sister.

let CNLabelContactRelationAuntParentsElderSister: String

The label for the contact’s parent’s elder sister.

let CNLabelContactRelationAuntParentsSister: String

The label for the contact’s parent’s sister.

let CNLabelContactRelationAuntParentsYoungerSister: String

The label for the contact’s parent’s younger sister.

let CNLabelContactRelationCousin: String

The label for the contact’s cousin.

let CNLabelContactRelationCousinFathersBrothersDaughter: String

The label for the contact’s father’s brother’s daughter.

let CNLabelContactRelationCousinFathersBrothersSon: String

The label for the contact’s father’s brother’s son.

let CNLabelContactRelationCousinFathersSistersDaughter: String

The label for the contact’s father’s sister’s daughter.

let CNLabelContactRelationCousinFathersSistersSon: String

The label for the contact’s father’s sister’s son.

let CNLabelContactRelationCousinGrandparentsSiblingsChild: String

The label for the contact’s grandparent’s sibling’s child.

let CNLabelContactRelationCousinGrandparentsSiblingsDaughter: String

The label for the contact’s grandparent’s sibling’s daughter.

let CNLabelContactRelationCousinGrandparentsSiblingsSon: String

The label for the contact’s grandparent’s sibling’s son.

let CNLabelContactRelationCousinMothersBrothersDaughter: String

The label for the contact’s mother’s brother’s daughter.

let CNLabelContactRelationCousinMothersBrothersSon: String

The label for the contact’s mother’s brother’s son.

let CNLabelContactRelationCousinMothersSistersDaughter: String

The label for the contact’s mother’s sister’s daughter.

let CNLabelContactRelationCousinMothersSistersSon: String

The label for the contact’s mother’s sister’s son.

let CNLabelContactRelationCousinOrSiblingsChild: String

The label for the contact’s cousin’s or sibling’s child.

let CNLabelContactRelationCousinParentsSiblingsChild: String

The label for the contact’s parent’s sibling’s child.

let CNLabelContactRelationCousinParentsSiblingsDaughter: String

The label for the contact’s parent’s sibling’s daughter.

let CNLabelContactRelationCousinParentsSiblingsSon: String

The label for the contact’s parent’s sibling’s son.

let CNLabelContactRelationDaughterInLaw: String

The label for the contact’s daughter-in-law.

let CNLabelContactRelationDaughterInLawOrSisterInLaw: String

The label for the contact’s daughter-in-law or sister-in-law.

let CNLabelContactRelationDaughterInLawOrStepdaughter: String

The label for the contact’s daughter-in-law or stepdaughter.

let CNLabelContactRelationElderCousin: String

The label for the contact’s elder cousin.

let CNLabelContactRelationElderCousinFathersBrothersDaughter: String

The label for the contact’s father’s brother’s daughter.

let CNLabelContactRelationElderCousinFathersBrothersSon: String

The label for the contact’s father’s brother’s son.

let CNLabelContactRelationElderCousinFathersSistersDaughter: String

The label for the contact’s father’s sister’s daughter.

let CNLabelContactRelationElderCousinFathersSistersSon: String

The label for the contact’s father’s sister’s son.

let CNLabelContactRelationElderCousinMothersBrothersDaughter: String

The label for the contact’s mother’s brother’s daughter.

let CNLabelContactRelationElderCousinMothersBrothersSon: String

The label for the contact’s mother’s brother’s son.

let CNLabelContactRelationElderCousinMothersSiblingsDaughterOrFathersSistersDaughter: String

The label for the contact’s mother’s sibling’s daughter or father’s sister’s daughter.

let CNLabelContactRelationElderCousinMothersSiblingsSonOrFathersSistersSon: String

The label for the contact’s mother’s sibling’s son or father’s sister’s son.

let CNLabelContactRelationElderCousinMothersSistersDaughter: String

The label for the contact’s mother’s sister’s daughter.

let CNLabelContactRelationElderCousinMothersSistersSon: String

The label for the contact’s mother’s sister’s son.

let CNLabelContactRelationElderCousinParentsSiblingsDaughter: String

The label for the contact’s parent’s sibling’s daughter.

let CNLabelContactRelationElderCousinParentsSiblingsSon: String

The label for the contact’s parent’s sibling’s son.

let CNLabelContactRelationFemaleCousin: String

The label for the contact’s female cousin.

let CNLabelContactRelationGrandaunt: String

The label for the contact’s grandaunt.

let CNLabelContactRelationGrandchild: String

The label for the contact’s grandchild.

let CNLabelContactRelationGrandchildOrSiblingsChild: String

The label for the contact’s grandchild or sibling’s child.

let CNLabelContactRelationGranddaughter: String

The label for the contact’s granddaughter.

let CNLabelContactRelationGranddaughterDaughtersDaughter: String

The label for the contact’s daughter’s daughter.

let CNLabelContactRelationGranddaughterSonsDaughter: String

The label for the contact’s son’s daughter.

let CNLabelContactRelationGranddaughterOrNiece: String

The label for the contact’s granddaughter or niece.

let CNLabelContactRelationGrandfather: String

The label for the contact’s grandfather.

let CNLabelContactRelationGrandfatherFathersFather: String

The label for the contact’s father’s father.

let CNLabelContactRelationGrandfatherMothersFather: String

The label for the contact’s mother’s father.

let CNLabelContactRelationGrandmother: String

The label for the contact’s grandmother.

let CNLabelContactRelationGrandmotherFathersMother: String

The label for the contact’s father’s mother.

let CNLabelContactRelationGrandmotherMothersMother: String

The label for the contact’s mother’s mother.

let CNLabelContactRelationGrandnephew: String

The label for the contact’s grandnephew.

let CNLabelContactRelationGrandnephewBrothersGrandson: String

The label for the contact’s brother’s grandson.

let CNLabelContactRelationGrandnephewSistersGrandson: String

The label for the contact’s sister’s grandson.

let CNLabelContactRelationGrandniece: String

The label for the contact’s grandniece.

let CNLabelContactRelationGrandnieceBrothersGranddaughter: String

The label for the contact’s brother’s granddaughter.

let CNLabelContactRelationGrandnieceSistersGranddaughter: String

The label for the contact’s sister’s granddaughter.

let CNLabelContactRelationGrandparent: String

The label for the contact’s grandparent.

let CNLabelContactRelationGrandson: String

The label for the contact’s grandson.

let CNLabelContactRelationGrandsonDaughtersSon: String

The label for the contact’s daughter’s son.

let CNLabelContactRelationGrandsonSonsSon: String

The label for the contact’s son’s son.

let CNLabelContactRelationGrandsonOrNephew: String

The label for the contact’s grandson or nephew.

let CNLabelContactRelationGranduncle: String

The label for the contact’s granduncle.

let CNLabelContactRelationGreatGrandchild: String

The label for the contact’s grandchild.

let CNLabelContactRelationGreatGrandchildOrSiblingsGrandchild: String

The label for the contact’s grandchild or sibling’s grandchild.

let CNLabelContactRelationGreatGranddaughter: String

The label for the contact’s great-granddaughter.

let CNLabelContactRelationGreatGrandfather: String

The label for the contact’s great-grandfather.

let CNLabelContactRelationGreatGrandmother: String

The label for the contact’s great-grandmother.

let CNLabelContactRelationGreatGrandparent: String

The label for the contact’s great-grandparent.

let CNLabelContactRelationGreatGrandson: String

The label for the contact’s great-grandson.

let CNLabelContactRelationMaleCousin: String

The label for the contact’s male cousin.

let CNLabelContactRelationNephew: String

The label for the contact’s nephew.

let CNLabelContactRelationNephewBrothersSon: String

The label for the contact’s brother’s son.

let CNLabelContactRelationNephewBrothersSonOrHusbandsSiblingsSon: String

The label for the contact’s brother’s son or husband’s sibling’s son.

let CNLabelContactRelationNephewOrCousin: String

The label for the contact’s nephew or cousin.

let CNLabelContactRelationNephewSistersSon: String

The label for the contact’s sister’s son.

let CNLabelContactRelationNephewSistersSonOrWifesSiblingsSon: String

The label for the contact’s sister’s son or wife’s sibling’s son.

let CNLabelContactRelationNiece: String

The label for the contact’s niece.

let CNLabelContactRelationNieceBrothersDaughter: String

The label for the contact’s brother’s daughter.

let CNLabelContactRelationNieceBrothersDaughterOrHusbandsSiblingsDaughter: String

The label for the contact’s brother’s daughter or husband’s sibling’s daughter.

let CNLabelContactRelationNieceOrCousin: String

The label for the contact’s niece or cousin.

let CNLabelContactRelationNieceSistersDaughter: String

The label for the contact’s sister’s daughter.

let CNLabelContactRelationNieceSistersDaughterOrWifesSiblingsDaughter: String

The label for the contact’s sister’s daughter or wife’s sibling’s daughter.

let CNLabelContactRelationParentsElderSibling: String

The label for the contact’s parent’s elder sibling.

let CNLabelContactRelationParentsSibling: String

The label for the contact’s parent’s sibling.

let CNLabelContactRelationParentsSiblingFathersElderSibling: String

The label for the contact’s father’s elder sibling.

let CNLabelContactRelationParentsSiblingFathersSibling: String

The label for the contact’s father’s sibling.

let CNLabelContactRelationParentsSiblingFathersYoungerSibling: String

The label for the contact’s father’s youngest sibling.

let CNLabelContactRelationParentsSiblingMothersElderSibling: String

The label for the contact’s mother’s elder sibling.

let CNLabelContactRelationParentsSiblingMothersSibling: String

The label for the contact’s mother’s sibling.

let CNLabelContactRelationParentsSiblingMothersYoungerSibling: String

The label for the contact’s mother’s younger sibling.

let CNLabelContactRelationParentsYoungerSibling: String

The label for the contact’s parent’s younger sibling.

let CNLabelContactRelationSiblingsChild: String

The label for the contact’s sibling’s child.

let CNLabelContactRelationSonInLaw: String

The label for the contact’s son-in-law.

let CNLabelContactRelationSonInLawOrBrotherInLaw: String

The label for the contact’s son-in-law or brother-in-law.

let CNLabelContactRelationSonInLawOrStepson: String

The label for the contact’s son-in-law or stepson.

let CNLabelContactRelationUncle: String

The label for the contact’s uncle.

let CNLabelContactRelationUncleFathersBrother: String

The label for the contact’s father’s brother.

let CNLabelContactRelationUncleFathersElderBrother: String

The label for the contact’s father’s elder brother.

let CNLabelContactRelationUncleFathersElderSistersHusband: String

The label for the contact’s elder sister’s husband.

let CNLabelContactRelationUncleFathersSistersHusband: String

The label for the contact’s father’s sister’s husband.

let CNLabelContactRelationUncleFathersYoungerBrother: String

The label for the contact’s father’s younger brother.

let CNLabelContactRelationUncleFathersYoungerSistersHusband: String

The label for the contact’s father’s younger sister’s husband.

let CNLabelContactRelationUncleMothersBrother: String

The label for the contact’s mother’s brother.

let CNLabelContactRelationUncleMothersElderBrother: String

The label for the contact’s mother’s elder brother.

let CNLabelContactRelationUncleMothersSistersHusband: String

The label for the contact’s mother’s sister’s husband.

let CNLabelContactRelationUncleMothersYoungerBrother: String

The label for the contact’s mother’s younger brother.

let CNLabelContactRelationUncleParentsBrother: String

The label for the contact’s parent’s brother.

let CNLabelContactRelationUncleParentsElderBrother: String

The label for the contact’s parent’s elder brother.

let CNLabelContactRelationUncleParentsYoungerBrother: String

The label for the contact’s parent’s younger brother.

let CNLabelContactRelationYoungerCousin: String

The label for the contact’s younger cousin.

let CNLabelContactRelationYoungerCousinFathersBrothersDaughter: String

The label for the contact’s father’s brother’s younger daughter.

let CNLabelContactRelationYoungerCousinFathersBrothersSon: String

The label for the contact’s father’s brother’s younger son.

let CNLabelContactRelationYoungerCousinFathersSistersDaughter: String

The label for the contact’s father’s sister’s younger daughter.

let CNLabelContactRelationYoungerCousinFathersSistersSon: String

The label for the contact’s father’s sister’s younger son.

let CNLabelContactRelationYoungerCousinMothersBrothersDaughter: String

The label for the contact’s mother’s brother’s younger daughter.

let CNLabelContactRelationYoungerCousinMothersBrothersSon: String

The label for the contact’s mother’s brother’s younger son.

let CNLabelContactRelationYoungerCousinMothersSiblingsDaughterOrFathersSistersDaughter: String

The label for the contact’s mother’s sibling’s younger daughter or father’s sister’s younger daughter.

let CNLabelContactRelationYoungerCousinMothersSiblingsSonOrFathersSistersSon: String

The label for the contact’s mother’s sibling’s younger son or father’s sister’s younger son.

let CNLabelContactRelationYoungerCousinMothersSistersDaughter: String

The label for the contact’s mother’s sister’s younger daughter.

let CNLabelContactRelationYoungerCousinMothersSistersSon: String

The label for the contact’s mother’s sister’s younger son.

let CNLabelContactRelationYoungerCousinParentsSiblingsDaughter: String

The label for the contact’s parent’s sibling’s younger daughter.

let CNLabelContactRelationYoungerCousinParentsSiblingsSon: String

The label for the contact’s parent’s sibling’s younger son.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Generic Types

class CNContactProperty

An object that represents a property of a contact.

