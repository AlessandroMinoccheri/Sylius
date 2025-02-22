# CHANGELOG FOR `1.11.X`

## v1.11.0-ALPHA.1 (2021-12-14)

#### TL;DR

- NEW FEATURE 🎉🎉🎉 Catalog promotions management: CRUD, asynchronous application on variants, different scopes, priorities management, exclusiveness and many more
- New API improvements: especially the **Shop** part, reaching ~80% of UI features coverage
- Bump required PHP version to 8.0, due to the end of life of PHP 7.4
- Bump required Symfony version to 5.4 LTS

#### Details

- [#12029](https://github.com/Sylius/Sylius/issues/12029) [BC BREAK] [API][BC-Break] Move commands and handlers to common namespace ([@lchrusciel](https://github.com/lchrusciel))
- [#12177](https://github.com/Sylius/Sylius/issues/12177) [Behat][API] Programitically generate API autorization token ([@lchrusciel](https://github.com/lchrusciel))
- [#12202](https://github.com/Sylius/Sylius/issues/12202) Feat: Add breadcrumb var in CRUD template for AdminBundle ([@toofff](https://github.com/toofff))
- [#12689](https://github.com/Sylius/Sylius/issues/12689) [API][Country] Initialize contract tests for api/v2 ([@GSadee](https://github.com/GSadee))
- [#12693](https://github.com/Sylius/Sylius/issues/12693) [API] allow extending and overwrite api in yaml + test ([@SirDomin](https://github.com/SirDomin))
- [#12695](https://github.com/Sylius/Sylius/issues/12695) [API][PaymentMethod] Add contract test for available payment methods endpoint ([@GSadee](https://github.com/GSadee))
- [#12700](https://github.com/Sylius/Sylius/issues/12700) [Docs] Docs customization ([@SirDomin](https://github.com/SirDomin))
- [#12703](https://github.com/Sylius/Sylius/issues/12703) [Api] Denying usage of unexisting promotion coupon ([@Tomanhez](https://github.com/Tomanhez))
- [#12704](https://github.com/Sylius/Sylius/issues/12704) [API] Denying usage of coupon for invalid promotion ([@Zales0123](https://github.com/Zales0123))
- [#12713](https://github.com/Sylius/Sylius/issues/12713) [API] Use serializer instead of custom view for shipping methods ([@GSadee](https://github.com/GSadee))
- [#12716](https://github.com/Sylius/Sylius/issues/12716) [API][ShippingMethod] Add contract test for available shipping methods endpoint ([@GSadee](https://github.com/GSadee))
- [#12718](https://github.com/Sylius/Sylius/issues/12718) [POC] Add change of tax by address ([@arti0090](https://github.com/arti0090))
- [#12719](https://github.com/Sylius/Sylius/issues/12719) [Api] Unnecessary addresses should not be saved to the database while addressing an order ([@Tomanhez](https://github.com/Tomanhez))
- [#12742](https://github.com/Sylius/Sylius/issues/12742) [API] Serialize only shipment id and method as shipment in order response ([@GSadee](https://github.com/GSadee))
- [#12743](https://github.com/Sylius/Sylius/issues/12743) [API] add final to clssess, cs fixes ([@SirDomin](https://github.com/SirDomin))
- [#12744](https://github.com/Sylius/Sylius/issues/12744) [Docs] fix unsetting filters ([@SirDomin](https://github.com/SirDomin))
- [#12745](https://github.com/Sylius/Sylius/issues/12745) [API] Add contract test to admin ProductVariant ([@arti0090](https://github.com/arti0090))
- [#12746](https://github.com/Sylius/Sylius/issues/12746) [API] handle shipping without addressing ([@SirDomin](https://github.com/SirDomin))
- [#12749](https://github.com/Sylius/Sylius/issues/12749) [API] change error to violation ([@SirDomin](https://github.com/SirDomin))
- [#12750](https://github.com/Sylius/Sylius/issues/12750) [ApiBundle] Small CS fixes ([@Zales0123](https://github.com/Zales0123))
- [#12761](https://github.com/Sylius/Sylius/issues/12761) [API] contract test for get order collection by guest ([@AdamKasp](https://github.com/AdamKasp))
- [#12766](https://github.com/Sylius/Sylius/issues/12766) [Locale]Available locales in channel by api ([@AdamKasp](https://github.com/AdamKasp))
- [#12769](https://github.com/Sylius/Sylius/issues/12769) [API] Refactor converting arguments of commands from IRIs to identifiers ([@Tomanhez](https://github.com/Tomanhez), [@GSadee](https://github.com/GSadee))
- [#12772](https://github.com/Sylius/Sylius/issues/12772) [ENHANCEMENT][API] Refactor Api Constraints to match rest of them ([@arti0090](https://github.com/arti0090))
- [#12774](https://github.com/Sylius/Sylius/issues/12774) [API] Add Product Image type to responses ([@arti0090](https://github.com/arti0090))
- [#12780](https://github.com/Sylius/Sylius/issues/12780) [Locale ][Api] Get locale refactor api ([@AdamKasp](https://github.com/AdamKasp))
- [#12782](https://github.com/Sylius/Sylius/issues/12782) [API] Check payment amount ([@Tomanhez](https://github.com/Tomanhez), [@AdamKasp](https://github.com/AdamKasp), [@GSadee](https://github.com/GSadee))
- [#12785](https://github.com/Sylius/Sylius/issues/12785) [API] Remove customer and serialize posted address ([@arti0090](https://github.com/arti0090))
- [#12790](https://github.com/Sylius/Sylius/issues/12790) [ENH][API] Fixing naming issues after PR for serializing post on address ([@arti0090](https://github.com/arti0090))
- [#12805](https://github.com/Sylius/Sylius/issues/12805) [Behat][API][Taxes] Turn on chunk of taxation related scenarios ([@lchrusciel](https://github.com/lchrusciel))
- [#12806](https://github.com/Sylius/Sylius/issues/12806) [Behat][API][Promotion] Turn on chunk of promotion scenarios ([@lchrusciel](https://github.com/lchrusciel))
- [#12830](https://github.com/Sylius/Sylius/issues/12830) [API] Exclude meaningless scenarios ([@lchrusciel](https://github.com/lchrusciel))
- [#12834](https://github.com/Sylius/Sylius/issues/12834) [Docs] Customization docs + yaml customization ([@SirDomin](https://github.com/SirDomin))
- [#12841](https://github.com/Sylius/Sylius/issues/12841) [UPGRADE] Split API and non API upgrade files ([@lchrusciel](https://github.com/lchrusciel))
- [#12842](https://github.com/Sylius/Sylius/issues/12842) [AUTO] Updated translations from Crowdin (master) ()
- [#12846](https://github.com/Sylius/Sylius/issues/12846) [BC BREAK] [API] Unification of filtration namespaces ([@lchrusciel](https://github.com/lchrusciel))
- [#12847](https://github.com/Sylius/Sylius/issues/12847) [API]Product image handling ([@arti0090](https://github.com/arti0090))
- [#12851](https://github.com/Sylius/Sylius/issues/12851) [Order] Protect processors from execution if the order is in a state different than cart ([@GSadee](https://github.com/GSadee))
- [#12854](https://github.com/Sylius/Sylius/issues/12854) [SM] Change priorities of State Machine callbacks ([@arti0090](https://github.com/arti0090))
- [#12855](https://github.com/Sylius/Sylius/issues/12855) [API][Country] Improve endpoints serialization ([@GSadee](https://github.com/GSadee))
- [#12856](https://github.com/Sylius/Sylius/issues/12856) [API] reduce customer update serialization ([@SirDomin](https://github.com/SirDomin))
- [#12858](https://github.com/Sylius/Sylius/issues/12858) [Core] Wrap resource update operation with a transaction ([@GSadee](https://github.com/GSadee))
- [#12862](https://github.com/Sylius/Sylius/issues/12862) [API] Add liip image filters to API ([@arti0090](https://github.com/arti0090), [@SirDomin](https://github.com/SirDomin))
- [#12866](https://github.com/Sylius/Sylius/issues/12866) Update release-cycle.rst ([@oallain](https://github.com/oallain))
- [#12874](https://github.com/Sylius/Sylius/issues/12874) [ORM] add created at index to customer ([@SirDomin](https://github.com/SirDomin))
- [#12876](https://github.com/Sylius/Sylius/issues/12876) [Minor] Add missing license blocks ([@lchrusciel](https://github.com/lchrusciel))
- [#12877](https://github.com/Sylius/Sylius/issues/12877) [API] add original price to product variant ([@SirDomin](https://github.com/SirDomin))
- [#12879](https://github.com/Sylius/Sylius/issues/12879) [DOCS] How to modify invoices ([@arti0090](https://github.com/arti0090))
- [#12880](https://github.com/Sylius/Sylius/issues/12880) [Maintenance] Configure builds on postgressql & mariadb ([@Arminek](https://github.com/Arminek))
- [#12883](https://github.com/Sylius/Sylius/issues/12883) [API] Rename original_price to originalPrice in api responses ([@AdamKasp](https://github.com/AdamKasp), [@arti0090](https://github.com/arti0090))
- [#12884](https://github.com/Sylius/Sylius/issues/12884) [Docs] add registration/login examples ([@SirDomin](https://github.com/SirDomin), [@arti0090](https://github.com/arti0090))
- [#12887](https://github.com/Sylius/Sylius/issues/12887) [DOCS] Generating invoice after payment ([@arti0090](https://github.com/arti0090))
- [#12888](https://github.com/Sylius/Sylius/issues/12888) [API] Fix formating for list in invoice cookbook ([@arti0090](https://github.com/arti0090))
- [#12889](https://github.com/Sylius/Sylius/issues/12889) Original price behat fix ([@arti0090](https://github.com/arti0090))
- [#12890](https://github.com/Sylius/Sylius/issues/12890) Fix to ordered list ([@arti0090](https://github.com/arti0090))
- [#12963](https://github.com/Sylius/Sylius/issues/12963) Update swagger docs with product variants originalPrice ([@arti0090](https://github.com/arti0090))
- [#12967](https://github.com/Sylius/Sylius/issues/12967) [API] Log in contract tests + minor fixes ([@lchrusciel](https://github.com/lchrusciel))
- [#12968](https://github.com/Sylius/Sylius/issues/12968) [API] AddressOrderHandler refactored to use customer provider ([@lchrusciel](https://github.com/lchrusciel))
- [#12969](https://github.com/Sylius/Sylius/issues/12969) [Maintenance] Dead code removal ([@lchrusciel](https://github.com/lchrusciel))
- [#12970](https://github.com/Sylius/Sylius/issues/12970) [DX] Add sylius prefixes to normalizers ALREADY_CALLED consts values to avoid name collision ([@lchrusciel](https://github.com/lchrusciel))
- [#12971](https://github.com/Sylius/Sylius/issues/12971) [DX] Adjust service names in ApiBundle ([@lchrusciel](https://github.com/lchrusciel))
- [#12972](https://github.com/Sylius/Sylius/issues/12972) [DOCS] Update images in api authorization book ([@arti0090](https://github.com/arti0090))
- [#12974](https://github.com/Sylius/Sylius/issues/12974) [Maintenance] Make all API Bundle services public and unify public notation ([@lchrusciel](https://github.com/lchrusciel))
- [#12978](https://github.com/Sylius/Sylius/issues/12978) [API] Resend verification email refactor to take current user from the security context ([@lchrusciel](https://github.com/lchrusciel))
- [#12979](https://github.com/Sylius/Sylius/issues/12979) [Minor] Adjust test class names to follow emerged convention ([@lchrusciel](https://github.com/lchrusciel))
- [#12980](https://github.com/Sylius/Sylius/issues/12980) [API] Expose taxon children as IRI in menu endpoint ([@lchrusciel](https://github.com/lchrusciel))
- [#12981](https://github.com/Sylius/Sylius/issues/12981) [API] Refactor current customer email aware commands ([@lchrusciel](https://github.com/lchrusciel))
- [#12983](https://github.com/Sylius/Sylius/issues/12983) [Documentation] Change the order of pages in Getting Started section ([@GSadee](https://github.com/GSadee))
- [#12986](https://github.com/Sylius/Sylius/issues/12986) [CatalogPromotion] Creating simple catalog promotion only with code and name ([@Arminek](https://github.com/Arminek), [@Tomanhez](https://github.com/Tomanhez))
- [#12990](https://github.com/Sylius/Sylius/issues/12990) [CatalogPromotions] Catalog promotion event ([@Tomanhez](https://github.com/Tomanhez), [@Arminek](https://github.com/Arminek))
- [#12994](https://github.com/Sylius/Sylius/issues/12994) Get, Update, Post and delete catalog promotions ([@arti0090](https://github.com/arti0090))
- [#12997](https://github.com/Sylius/Sylius/issues/12997) [API] Add gender field to customer ([@arti0090](https://github.com/arti0090))
- [#12998](https://github.com/Sylius/Sylius/issues/12998) [CatalogPromotion][API] Minor fixes to creating simple catalog promotion ([@GSadee](https://github.com/GSadee))
- [#13001](https://github.com/Sylius/Sylius/issues/13001) [Catalog Promotions] add rule to catalog promotion ([@AdamKasp](https://github.com/AdamKasp), [@SirDomin](https://github.com/SirDomin))
- [#13002](https://github.com/Sylius/Sylius/issues/13002) [CatalogPromotion] Applying Catalog Promotion with hardcoded rule and action ([@Tomanhez](https://github.com/Tomanhez), [@Zales0123](https://github.com/Zales0123))
- [#13003](https://github.com/Sylius/Sylius/issues/13003) Fixes to endpoints and contract tests of CP ([@arti0090](https://github.com/arti0090))
- [#13005](https://github.com/Sylius/Sylius/issues/13005) [CatalogPromotion][API] Create catalog promotion with translatable fields ([@GSadee](https://github.com/GSadee))
- [#13008](https://github.com/Sylius/Sylius/issues/13008) [Catalog Promotions] Add behat scenarios for endpoints ([@arti0090](https://github.com/arti0090))
- [#13009](https://github.com/Sylius/Sylius/issues/13009) [CatalogPromotion][API] Add channels to catalog promotion ([@GSadee](https://github.com/GSadee))
- [#13010](https://github.com/Sylius/Sylius/issues/13010) [Catalog Promotion] Remove delete endpoint ([@arti0090](https://github.com/arti0090))
- [#13011](https://github.com/Sylius/Sylius/issues/13011) [CatalogPromotion][API] Add simple validation for creating catalog promotion ([@GSadee](https://github.com/GSadee))
- [#13013](https://github.com/Sylius/Sylius/issues/13013) [CatalogPromotion][API] Extend the possibility of editing catalog promotion ([@GSadee](https://github.com/GSadee))
- [#13014](https://github.com/Sylius/Sylius/issues/13014) [CatalogPromotion] Use Catalog Promotion rule during application ([@Zales0123](https://github.com/Zales0123))
- [#13015](https://github.com/Sylius/Sylius/issues/13015) [CatalogPromotion] Add fixtures for catalog promotion entity ([@GSadee](https://github.com/GSadee))
- [#13016](https://github.com/Sylius/Sylius/issues/13016) [CatalogPromotion][Behat] Minor improvements for catalog promotions scenarios ([@GSadee](https://github.com/GSadee))
- [#13017](https://github.com/Sylius/Sylius/issues/13017) [CatalogPromotion][API] Add scenarios for browsing catalog promotions ([@GSadee](https://github.com/GSadee))
- [#13022](https://github.com/Sylius/Sylius/issues/13022) [Bug] Fix default sylius config file path in Sylius master branch ([@lchrusciel](https://github.com/lchrusciel))
- [#13026](https://github.com/Sylius/Sylius/issues/13026) [CatalogPromotion][Admin] Add browsing catalog promotions ([@GSadee](https://github.com/GSadee))
- [#13028](https://github.com/Sylius/Sylius/issues/13028) [CatalogPromotion][Admin] Add creating catalog promotion ([@GSadee](https://github.com/GSadee))
- [#13029](https://github.com/Sylius/Sylius/issues/13029) Catalog promotions action ([@SirDomin](https://github.com/SirDomin), [@Zales0123](https://github.com/Zales0123))
- [#13030](https://github.com/Sylius/Sylius/issues/13030) Add validation for Catalog Promotion Rules ([@AdamKasp](https://github.com/AdamKasp))
- [#13033](https://github.com/Sylius/Sylius/issues/13033) [Catalog Promotion] refactor rule configuration change iri with code ([@AdamKasp](https://github.com/AdamKasp))
- [#13034](https://github.com/Sylius/Sylius/issues/13034) [CatalogPromotion][Admin] Add editing catalog promotions ([@GSadee](https://github.com/GSadee))
- [#13035](https://github.com/Sylius/Sylius/issues/13035) [CatalogPromotions] Inform about promotions applied on variants ([@Zales0123](https://github.com/Zales0123))
- [#13036](https://github.com/Sylius/Sylius/issues/13036) [CatalogPromotions] Use actions for discount application ([@Zales0123](https://github.com/Zales0123))
- [#13041](https://github.com/Sylius/Sylius/issues/13041) [CartPromotion][Admin] Change label of promotion to cart promotion ([@GSadee](https://github.com/GSadee))
- [#13048](https://github.com/Sylius/Sylius/issues/13048) [CatalogPromotions] Move variant-related CatalogPromotionRule constant to Core ([@Zales0123](https://github.com/Zales0123))
- [#13052](https://github.com/Sylius/Sylius/issues/13052) [CatalogPromotions] Manage rules and actions from UI ([@Zales0123](https://github.com/Zales0123))
- [#13055](https://github.com/Sylius/Sylius/issues/13055) [CatalogPromotions] Add fixtures for catalog promotions rules and actions ([@Tomanhez](https://github.com/Tomanhez))
- [#13060](https://github.com/Sylius/Sylius/issues/13060) [CP] Add scenario for `Inform about promotions applied on variant` ([@arti0090](https://github.com/arti0090))
- [#13061](https://github.com/Sylius/Sylius/issues/13061) [UI][Behat] tests for editing catalog promotion with rule and action ([@SirDomin](https://github.com/SirDomin))
- [#13064](https://github.com/Sylius/Sylius/issues/13064) [Behat] move actions redirect to different step ([@SirDomin](https://github.com/SirDomin))
- [#13066](https://github.com/Sylius/Sylius/issues/13066) [CatalogPromotion] refactor cp rule to be consistent with cp action ([@SirDomin](https://github.com/SirDomin))
- [#13067](https://github.com/Sylius/Sylius/issues/13067) Fix persisting of Catalog Promotion data on create ([@arti0090](https://github.com/arti0090))
- [#13068](https://github.com/Sylius/Sylius/issues/13068) [CatalogPromotions][Api] Add test for creation rule ([@Tomanhez](https://github.com/Tomanhez))
- [#13071](https://github.com/Sylius/Sylius/issues/13071) [CatalogPromotion][API] Add validation for creating catalog promotion with actions ([@Arminek](https://github.com/Arminek), [@GSadee](https://github.com/GSadee))
- [#13072](https://github.com/Sylius/Sylius/issues/13072) [CatalogPromotion] Improve names and namespaces of catalog promotion rule form types ([@GSadee](https://github.com/GSadee))
- [#13073](https://github.com/Sylius/Sylius/issues/13073) [CatalogPromotion][Behat] Improve steps names ([@GSadee](https://github.com/GSadee))
- [#13075](https://github.com/Sylius/Sylius/issues/13075) [CatalogPromotion][API] Refactor validation of rules ([@GSadee](https://github.com/GSadee))
- [#13077](https://github.com/Sylius/Sylius/issues/13077) [CatalogPromotion] Fix configuration of fixtures for actions and rules ([@GSadee](https://github.com/GSadee))
- [#13079](https://github.com/Sylius/Sylius/issues/13079) [DOCS] Rename promotions to cart promotions ([@arti0090](https://github.com/arti0090))
- [#13080](https://github.com/Sylius/Sylius/issues/13080) [Catalog Promotions] Fixing issues with multiple variants ([@arti0090](https://github.com/arti0090))
- [#13081](https://github.com/Sylius/Sylius/issues/13081) [CatalogPromotion][API] Apply catalog promotion in proper channels ([@GSadee](https://github.com/GSadee))
- [#13082](https://github.com/Sylius/Sylius/issues/13082) [API] [Catalog Promotion] validate action amount ([@AdamKasp](https://github.com/AdamKasp))
- [#13084](https://github.com/Sylius/Sylius/issues/13084) [DOCS]Add Catalog Promotion documentation ([@arti0090](https://github.com/arti0090))
- [#13085](https://github.com/Sylius/Sylius/issues/13085) [CatalogPromotions] Modify AppliedPromotionInformationFormatter ([@Tomanhez](https://github.com/Tomanhez))
- [#13086](https://github.com/Sylius/Sylius/issues/13086) [CatalogPromotion][API] Add examples of rules and actions to Swagger ([@GSadee](https://github.com/GSadee))
- [#13089](https://github.com/Sylius/Sylius/issues/13089) [CatalogPromotions] Add missing description to applied promotions ([@arti0090](https://github.com/arti0090))
- [#13091](https://github.com/Sylius/Sylius/issues/13091) [CatalogPromotions] Add api behat for multiple catalog promotions ([@Tomanhez](https://github.com/Tomanhez))
- [#13092](https://github.com/Sylius/Sylius/issues/13092) [CatalogPromotion][Behat] Add scenarios for reapplying catalog promotions after editing its channels ([@GSadee](https://github.com/GSadee))
- [#13093](https://github.com/Sylius/Sylius/issues/13093) [CatalogPromotions][Validation] add validation to catalog promotion, … ([@SirDomin](https://github.com/SirDomin))
- [#13094](https://github.com/Sylius/Sylius/issues/13094) [Catalog Promotions][Docs] Add a section about how promotions are applied ([@arti0090](https://github.com/arti0090))
- [#13096](https://github.com/Sylius/Sylius/issues/13096) [DOCS] Fix catalog promotions docs reference ([@arti0090](https://github.com/arti0090))
- [#13098](https://github.com/Sylius/Sylius/issues/13098) [CatalogPromotions] Add product to cart with discounted catalog price ([@Tomanhez](https://github.com/Tomanhez), [@arti0090](https://github.com/arti0090))
- [#13100](https://github.com/Sylius/Sylius/issues/13100) [CatalogPromotion] Clear applied catalog promotions after updating ([@GSadee](https://github.com/GSadee))
- [#13101](https://github.com/Sylius/Sylius/issues/13101) [CatalogPromotions] Showing catalog promotions in Products index and show page ([@SirDomin](https://github.com/SirDomin), [@Zales0123](https://github.com/Zales0123))
- [#13103](https://github.com/Sylius/Sylius/issues/13103) [UI][Catalog Promotion] Add discounted product to cart ([@AdamKasp](https://github.com/AdamKasp))
- [#13104](https://github.com/Sylius/Sylius/issues/13104) [API] Use POST action to add new item to cart ([@lchrusciel](https://github.com/lchrusciel))
- [#13105](https://github.com/Sylius/Sylius/issues/13105) [Catalog Promotions] Reapplying Catalog Promotion on Action Edit ([@arti0090](https://github.com/arti0090))
- [#13107](https://github.com/Sylius/Sylius/issues/13107) [Api] Customer add product with discounted catalog price ([@Tomanhez](https://github.com/Tomanhez))
- [#13110](https://github.com/Sylius/Sylius/issues/13110) [Fixtures] Extract promotions to a separate file to fix applying catalog promotions ([@GSadee](https://github.com/GSadee))
- [#13111](https://github.com/Sylius/Sylius/issues/13111) [ChannelPricing] Improve query for finding discounted pricings ([@GSadee](https://github.com/GSadee))
- [#13112](https://github.com/Sylius/Sylius/issues/13112) [Catalog Promotion] Cart catalog promotion becomes ineligible ([@GSadee](https://github.com/GSadee), [@AdamKasp](https://github.com/AdamKasp))
- [#13114](https://github.com/Sylius/Sylius/issues/13114) [CatalogPromotions] Do not display applied promotion description in label if not set ([@Zales0123](https://github.com/Zales0123))
- [#13117](https://github.com/Sylius/Sylius/issues/13117) [API] Remove phoneNumber from Customer command and handler ([@lchrusciel](https://github.com/lchrusciel))
- [#13121](https://github.com/Sylius/Sylius/issues/13121) [AUTO] Updated translations from Crowdin (master) ([@bot](https://github.com/bot)@[@sylius](https://github.com/sylius).[@org](https://github.com/org))
- [#13124](https://github.com/Sylius/Sylius/issues/13124) [CatalogPromotion][API] Reapplying catalog promotions after update its channel ([@AdamKasp](https://github.com/AdamKasp))
- [#13128](https://github.com/Sylius/Sylius/issues/13128) [API][CatalogPromotion] Reapplying catalog promotion on variant once its data changes ([@GSadee](https://github.com/GSadee))
- [#13129](https://github.com/Sylius/Sylius/issues/13129) [API][CatalogPromotion] Reapplying catalog promotions on rule update ([@SirDomin](https://github.com/SirDomin), [@GSadee](https://github.com/GSadee))
- [#13130](https://github.com/Sylius/Sylius/issues/13130) [CatalogPromotion][Behat] Cover scenarios for reapplying catalog promotions ([@Tomanhez](https://github.com/Tomanhez), [@GSadee](https://github.com/GSadee))
- [#13131](https://github.com/Sylius/Sylius/issues/13131) [CatalogPromotions][API] Reapply promotions after action removal ([@arti0090](https://github.com/arti0090))
- [#13132](https://github.com/Sylius/Sylius/issues/13132) [API][UI] Toggle catalog promotion ([@AdamKasp](https://github.com/AdamKasp))
- [#13133](https://github.com/Sylius/Sylius/issues/13133) Reorganize flushes in Catalog Promotions processing ([@Zales0123](https://github.com/Zales0123))
- [#13137](https://github.com/Sylius/Sylius/issues/13137) [CatalogPromotions] Add behats for CatalogPromotions based on taxon ([@Tomanhez](https://github.com/Tomanhez), [@AdamKasp](https://github.com/AdamKasp))
- [#13138](https://github.com/Sylius/Sylius/issues/13138) [Build] ignore string inflector phpstan ([@SirDomin](https://github.com/SirDomin))
- [#13141](https://github.com/Sylius/Sylius/issues/13141) [UI][CatalogPromotion] Reapplying catalog promotion on variant once its data changes ([@GSadee](https://github.com/GSadee))
- [#13145](https://github.com/Sylius/Sylius/issues/13145) [API][CatalogPromotion] refactor Variants Provider to strategy Pattern ([@AdamKasp](https://github.com/AdamKasp))
- [#13146](https://github.com/Sylius/Sylius/issues/13146) [Api] CatalogPromotionRule per taxon ([@AdamKasp](https://github.com/AdamKasp), [@Tomanhez](https://github.com/Tomanhez), [@Zales0123](https://github.com/Zales0123))
- [#13147](https://github.com/Sylius/Sylius/issues/13147) [API] Fix admin path in swagger ([@arti0090](https://github.com/arti0090))
- [#13150](https://github.com/Sylius/Sylius/issues/13150) [API] Refactor path removal with (unset) ([@Zales0123](https://github.com/Zales0123))
- [#13152](https://github.com/Sylius/Sylius/issues/13152) [CatalogPromotion] Refactor to not listen on Doctrine events ([@GSadee](https://github.com/GSadee))
- [#13153](https://github.com/Sylius/Sylius/issues/13153) [UI][CatalogPromotion] Reapply catalog promotions after editing their rules and actions ([@GSadee](https://github.com/GSadee))
- [#13155](https://github.com/Sylius/Sylius/issues/13155) [Documentation][CatalogPromotion] Adjust docs after removing usage of Doctrine events ([@GSadee](https://github.com/GSadee))
- [#13156](https://github.com/Sylius/Sylius/issues/13156) [CatalogPromotion] change change channel with toggle in UI ([@AdamKasp](https://github.com/AdamKasp))
- [#13161](https://github.com/Sylius/Sylius/issues/13161) [CatalogPromotions] Rename CP Rule to Scope ([@arti0090](https://github.com/arti0090))
- [#13164](https://github.com/Sylius/Sylius/issues/13164) Rename behat file from rule to scope on catalog promotion ([@arti0090](https://github.com/arti0090))
- [#13168](https://github.com/Sylius/Sylius/issues/13168) [CatalogPromotion] Minor fixes after renaming rule to scope ([@GSadee](https://github.com/GSadee))
- [#13169](https://github.com/Sylius/Sylius/issues/13169) [Catalog Promotions] Reapply CP after changing its taxons ([@arti0090](https://github.com/arti0090))
- [#13174](https://github.com/Sylius/Sylius/issues/13174) [CatalogPromotion] Refactor scope validators to be more extendable ([@GSadee](https://github.com/GSadee))
- [#13175](https://github.com/Sylius/Sylius/issues/13175) [CatalogPromotions] "For taxons" scope in UI with dynamic form configurations ([@Zales0123](https://github.com/Zales0123))
- [#13179](https://github.com/Sylius/Sylius/issues/13179) [CatalogPromotions] Start and end date  ([@Zales0123](https://github.com/Zales0123))
- [#13181](https://github.com/Sylius/Sylius/issues/13181) [CatalogPromotion][UI] Reapply catalog promotions after product's taxon changes + refactor ([@GSadee](https://github.com/GSadee))
- [#13182](https://github.com/Sylius/Sylius/issues/13182) [CatalogPromotions] Display taxons with names in scope ([@Zales0123](https://github.com/Zales0123))
- [#13183](https://github.com/Sylius/Sylius/issues/13183) [DOCS][Catalog Promotions] Making new CP scope ([@arti0090](https://github.com/arti0090))
- [#13184](https://github.com/Sylius/Sylius/issues/13184) [CatalogPromotion][UI][Behat] Implement scenarios for reapplying catalog promotions after editing their for taxons scope ([@GSadee](https://github.com/GSadee))
- [#13186](https://github.com/Sylius/Sylius/issues/13186) [CatalogPromotion][API][UI] Introduce states with state machine for catalog promotion ([@GSadee](https://github.com/GSadee))
- [#13189](https://github.com/Sylius/Sylius/issues/13189) [CatalogPromotions] Take into account CP dates during processing ([@Zales0123](https://github.com/Zales0123))
- [#13190](https://github.com/Sylius/Sylius/issues/13190) [CatalogPromotion] Minor improvements in EligibleCatalogPromotionsProvider ([@GSadee](https://github.com/GSadee))
- [#13191](https://github.com/Sylius/Sylius/issues/13191) [CatalogPromotion][Behat] Add scenario for applying catalog promotion with different scopes defined ([@GSadee](https://github.com/GSadee))
- [#13192](https://github.com/Sylius/Sylius/issues/13192) [DOCS] Refactor from promotion to cart promotion ([@arti0090](https://github.com/arti0090))
- [#13195](https://github.com/Sylius/Sylius/issues/13195) [CatalogPromotion] Secure that the catalog promotion cannot be edited ([@GSadee](https://github.com/GSadee))
- [#13196](https://github.com/Sylius/Sylius/issues/13196) [CatalogPromotions] async workers introduction ([@SirDomin](https://github.com/SirDomin))
- [#13206](https://github.com/Sylius/Sylius/issues/13206) [API][UI] Sort products by their discounted price ([@arti0090](https://github.com/arti0090), [@GSadee](https://github.com/GSadee))
- [#13208](https://github.com/Sylius/Sylius/issues/13208) [CatalogPromotion] fix pricing clearer ([@AdamKasp](https://github.com/AdamKasp))
- [#13209](https://github.com/Sylius/Sylius/issues/13209) Move channel pricing to separate tab ([@AdamKasp](https://github.com/AdamKasp))
- [#13212](https://github.com/Sylius/Sylius/issues/13212) [Hot-fix] Conflict doctrine/dbal 3.* in ApiBundle ([@Zales0123](https://github.com/Zales0123))
- [#13217](https://github.com/Sylius/Sylius/issues/13217) [Docs] Add description of prices ([@AdamKasp](https://github.com/AdamKasp))
- [#13218](https://github.com/Sylius/Sylius/issues/13218) [CatalogPromotion] Add show page for catalog promotion ([@GSadee](https://github.com/GSadee))
- [#13219](https://github.com/Sylius/Sylius/issues/13219) [ChannelPricing] fixes after merge ([@AdamKasp](https://github.com/AdamKasp))
- [#13220](https://github.com/Sylius/Sylius/issues/13220) Add note about time delay ([@AdamKasp](https://github.com/AdamKasp))
- [#13221](https://github.com/Sylius/Sylius/issues/13221) [CatalogPromotions] Prevent editing start and end date ([@Zales0123](https://github.com/Zales0123))
- [#13222](https://github.com/Sylius/Sylius/issues/13222) [UI][Catalog Promotions] Set default time for CP dates if not provided ([@Zales0123](https://github.com/Zales0123))
- [#13226](https://github.com/Sylius/Sylius/issues/13226) [CatalogPromotions] Handle failed catalog promotions ([@SirDomin](https://github.com/SirDomin))
- [#13227](https://github.com/Sylius/Sylius/issues/13227) [CatalogPromotions] Always prevent CP dates editing - even if they're not set during creation ([@Zales0123](https://github.com/Zales0123))
- [#13228](https://github.com/Sylius/Sylius/issues/13228) [Conflict] add conflict to new release of fos-rest ([@SirDomin](https://github.com/SirDomin))
- [#13229](https://github.com/Sylius/Sylius/issues/13229) [CatalogPromotion] docs about async messages ([@AdamKasp](https://github.com/AdamKasp))
- [#13230](https://github.com/Sylius/Sylius/issues/13230) [CatalogPromotion] change DateRange criteria + functional tests ([@SirDomin](https://github.com/SirDomin))
- [#13231](https://github.com/Sylius/Sylius/issues/13231) [CatalogPromotion] Make criteria services public in container by default ([@lchrusciel](https://github.com/lchrusciel))
- [#13234](https://github.com/Sylius/Sylius/issues/13234) Update Typo in Performance section ([@zairigimad](https://github.com/zairigimad))
- [#13235](https://github.com/Sylius/Sylius/issues/13235) [CatalogPromotion] Changing state after toggling catalog promotion ([@GSadee](https://github.com/GSadee))
- [#13236](https://github.com/Sylius/Sylius/issues/13236) [CatalogPromotion] fix service typo, stateMachine error fixed ([@SirDomin](https://github.com/SirDomin))
- [#13248](https://github.com/Sylius/Sylius/issues/13248) [CatalogPromotion] Small fixes to `docs about async messages` ([@arti0090](https://github.com/arti0090))
- [#13256](https://github.com/Sylius/Sylius/issues/13256) [CatalogPromotion] dates are editable and validated ([@AdamKasp](https://github.com/AdamKasp))
- [#13260](https://github.com/Sylius/Sylius/issues/13260) [CatalogPromotions] Add priorities ([@Zales0123](https://github.com/Zales0123), [@GSadee](https://github.com/GSadee))
- [#13262](https://github.com/Sylius/Sylius/issues/13262) Remove conflict with fos/rest-bundle ([@Zales0123](https://github.com/Zales0123))
- [#13264](https://github.com/Sylius/Sylius/issues/13264) [AUTO] Updated translations from Crowdin (master) ([@bot](https://github.com/bot)@[@sylius](https://github.com/sylius).[@org](https://github.com/org))
- [#13266](https://github.com/Sylius/Sylius/issues/13266) Specify minimum price of product and apply it on catalogPromotions ([@SirDomin](https://github.com/SirDomin))
- [#13271](https://github.com/Sylius/Sylius/issues/13271) Fix composer.json file after rebase ([@Zales0123](https://github.com/Zales0123))
- [#13273](https://github.com/Sylius/Sylius/issues/13273) [CatalogPromotion] Add "for products" scope ([@GSadee](https://github.com/GSadee))
- [#13279](https://github.com/Sylius/Sylius/issues/13279) [Behat] Remove deprecated whitespace from behat tags on master ([@GSadee](https://github.com/GSadee))
- [#13280](https://github.com/Sylius/Sylius/issues/13280) Get products by slug api endpoint ([@paullla](https://github.com/paullla))
- [#13287](https://github.com/Sylius/Sylius/issues/13287) List of channel currencies endpoint ([@paullla](https://github.com/paullla))
- [#13291](https://github.com/Sylius/Sylius/issues/13291) [MinimumPrice] Handle minimum price cart ([@SirDomin](https://github.com/SirDomin), [@lchrusciel](https://github.com/lchrusciel))
- [#13294](https://github.com/Sylius/Sylius/issues/13294) [Minimum Price] documentation ([@AdamKasp](https://github.com/AdamKasp))
- [#13295](https://github.com/Sylius/Sylius/issues/13295) [Github] clear cache before phpunit ([@SirDomin](https://github.com/SirDomin))
- [#13297](https://github.com/Sylius/Sylius/issues/13297) [Actions] disable xdebug for actions ([@SirDomin](https://github.com/SirDomin))
- [#13299](https://github.com/Sylius/Sylius/issues/13299) [Adr] Fix customization api documentation url ([@SebLours](https://github.com/SebLours))
- [#13303](https://github.com/Sylius/Sylius/issues/13303) [CatalogPromotion] Add exclusiveness flag ([@AdamKasp](https://github.com/AdamKasp))
- [#13305](https://github.com/Sylius/Sylius/issues/13305) [Behat] Skip ui based checkout steps in api coverage ([@lchrusciel](https://github.com/lchrusciel))
- [#13306](https://github.com/Sylius/Sylius/issues/13306) [Minor][Behat] Style and type refactor ([@lchrusciel](https://github.com/lchrusciel))
- [#13311](https://github.com/Sylius/Sylius/issues/13311) Code cleanup - user password reset ([@antonioperic](https://github.com/antonioperic))
- [#13325](https://github.com/Sylius/Sylius/issues/13325) [CatalogPromotion][API][UI] Fixed discount action ([@GSadee](https://github.com/GSadee))
- [#13328](https://github.com/Sylius/Sylius/issues/13328) [CartPromotion][API][UI] Apply on discounted flag added ([@SirDomin](https://github.com/SirDomin), [@AdamKasp](https://github.com/AdamKasp))
- [#13329](https://github.com/Sylius/Sylius/issues/13329) Addressing, locale update and apply coupon code unified to one endpoint ([@paullla](https://github.com/paullla))
- [#13333](https://github.com/Sylius/Sylius/issues/13333) Replace data providers with doctrine extensions ([@paullla](https://github.com/paullla))
- [#13337](https://github.com/Sylius/Sylius/issues/13337) [AUTO] Updated translations from Crowdin (master) ([@bot](https://github.com/bot)@[@sylius](https://github.com/sylius).[@org](https://github.com/org))
- [#13338](https://github.com/Sylius/Sylius/issues/13338) Drop support for PHP 7.4 ([@AdamKasp](https://github.com/AdamKasp))
- [#13339](https://github.com/Sylius/Sylius/issues/13339) Add Support for Symfony 5.4 ([@AdamKasp](https://github.com/AdamKasp))
- [#13343](https://github.com/Sylius/Sylius/issues/13343) [Documentation] Update required version of PHP ([@GSadee](https://github.com/GSadee))
- [#13344](https://github.com/Sylius/Sylius/issues/13344) Doctrine Extensions upgrade info & code cleanup ([@paullla](https://github.com/paullla))
- [#13349](https://github.com/Sylius/Sylius/issues/13349) [CartPromotion][CatalogPromotion] Receiving discount only on non discounted products ([@GSadee](https://github.com/GSadee), [@SirDomin](https://github.com/SirDomin))
- [#13350](https://github.com/Sylius/Sylius/issues/13350) Order items list and order/item adjustments serialization groups ([@paullla](https://github.com/paullla))
- [#13352](https://github.com/Sylius/Sylius/issues/13352) Use QueryNameGenerator for extension query parameters ([@paullla](https://github.com/paullla))
- [#13367](https://github.com/Sylius/Sylius/issues/13367) [Maintenance] Remove Sf6.0 conflicts ([@lchrusciel](https://github.com/lchrusciel))
- [#13368](https://github.com/Sylius/Sylius/issues/13368) [UI] change time format to 24H, autocomplete times on data change ([@SirDomin](https://github.com/SirDomin))
- [#13369](https://github.com/Sylius/Sylius/issues/13369) [Command] add command to generate jwt ([@SirDomin](https://github.com/SirDomin))
- [#13373](https://github.com/Sylius/Sylius/issues/13373) Revert "Move "polishsymfonycommunity/symfony-mocker-container" into dev dependencies" due to the BC break ([@lchrusciel](https://github.com/lchrusciel))
- [#13375](https://github.com/Sylius/Sylius/issues/13375) Catalog promotion channel pricing relation ([@Rafikooo](https://github.com/Rafikooo))
- [#13377](https://github.com/Sylius/Sylius/issues/13377) Move "polishsymfonycommunity/symfony-mocker-container" into dev dependencies ([@stloyd](https://github.com/stloyd), [@lchrusciel](https://github.com/lchrusciel))
- [#13378](https://github.com/Sylius/Sylius/issues/13378) [CatalogPromotion] change icon on show page ([@AdamKasp](https://github.com/AdamKasp))
- [#13380](https://github.com/Sylius/Sylius/issues/13380) [Bug][Migrations] Add missing mysql check for our migrations to ensure proper syntax is available - master edition ([@lchrusciel](https://github.com/lchrusciel))
- [#13381](https://github.com/Sylius/Sylius/issues/13381) Drop support for older `gedmo/doctrine-extensions` versions ([@mbabker](https://github.com/mbabker))
- [#13387](https://github.com/Sylius/Sylius/issues/13387) Explanation note about minimum price in product variant creation form ([@TheMilek](https://github.com/TheMilek))
- [#13388](https://github.com/Sylius/Sylius/issues/13388) [Migrations] Remove invalid NOT NULL usage ([@Zales0123](https://github.com/Zales0123))
- [#13391](https://github.com/Sylius/Sylius/issues/13391) [Maintenance] Conflict with Symfony 6 packages ([@lchrusciel](https://github.com/lchrusciel))
