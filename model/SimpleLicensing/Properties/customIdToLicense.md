SPDX-License-Identifier: Community-Spec-1.0

# customIdToLicense

## Summary

Maps a LicenseRef or AdditionRef string for a Custom License or a Custom
License Addition to a CustomLicense, a CustomLicenseAddition, or a
SimpleLicensingText

## Description

Within a License Expression, references can be made to a Custom License or a
Custom License Addition.

The [License Expression syntax](../../../annexes/spdx-license-expressions.md)
dictates any reference starting with a
"LicenseRef-" or "AdditionRef-" refers to license or addition text not found in
the official [SPDX License List](https://spdx.org/licenses/).

The key for the DictionaryEntry is the string used in the license expression
and the value is target Element, which must be a CustomLicense,
CustomLicenseAddition, or SimpleLicensingText.

## Metadata

- name: customIdToLicense
- Nature: ObjectProperty
- Range: /Core/ElementMap
