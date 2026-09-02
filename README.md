
# Medicine Guide Pakistan — Play Store Preparation v2.0

Included:
- 100+ curated medicine records focused on common Pakistani community-pharmacy therapeutic areas
- Urdu / English UI switch
- Search by brand, generic, category and indication
- Favorites saved locally
- Medicine detail screen
- Prescription (Rx) flag
- Safety warnings and medical disclaimer
- JSON database separated from app code for easier future updates

## Build
Install Flutter SDK, then:
flutter pub get
flutter run

For a release APK:
flutter build apk --release

For Google Play:
flutter build appbundle --release

The Play Store upload artifact is:
build/app/outputs/bundle/release/app-release.aab

## Critical verification before publishing
The database is a curated starter catalog, not a claim of "every medicine used in Pakistan" or a statistical ranking by unit volume. Pakistan's pharmaceutical market contains a very large number of registered products/brands.

DRAP maintains the official Registered Drugs Index and states that its registration data can include product/brand name, dosage form, active ingredients, registration number/date, marketing authorization holder and manufacturer. Verify every product record against the current DRAP registry and current approved product information before publishing.

Also verify:
- exact brand spelling and current registration status
- strength, dosage form, pack size and manufacturer
- adult/pediatric doses
- contraindications and drug interactions
- pregnancy/lactation warnings
- OTC/Rx classification and local legal requirements
- copyright/trademark permissions for brand names/logos and product images
- current Google Play medical-app policy, privacy requirements and Data Safety declarations

Do not ship dosing as a generic fixed recommendation when the dose depends on indication, age, weight, renal/hepatic function or other clinical factors.


## v3 expansion
The catalog now contains 158 records, including richer clinical-reference fields and pharmacist-review placeholders. See PHARMACIST_REVIEW_GUIDE.md.
