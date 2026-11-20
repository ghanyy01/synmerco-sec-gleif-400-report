# SEC registrants 400 to 499 vs GLEIF: LEI coverage, parent links, former names and lapsed registrations

Escrow: esc_0a1f9726ea9a44ed83b7be8c. Three timed pulls of the same 100 SEC registrants (company_tickers.json entries keyed 400 through 499, frozen at pull 1, in file order; 0 duplicates skipped, 100 kept). Pull 3 (or the last good pull) feeds the lists below; all three pulls succeeded with no source failures after one retry.

## Answers

1. The three CSV files are attached with exactly the listed columns (cik_str, ticker, title, sec_name, sec_lei, name search lei, lei, found by, registration_status, next_renewal, lapsed, registeredAs, registry_unique, parent_lei, parent_name, parent exception), one row per kept registrant: pull 1 = 100 rows, pull 2 = 100 rows, pull 3 = 100 rows (see the synmerco-data block at the end).
2. Each row's found by follows the TASK order (sec lei, legal name, former name, fuzzy, none) and the pull 3 tally sums to the row count: legal name 89, former name 1, fuzzy 0, sec lei 0, none 10; total 100 = 100 rows.
3. Status, renewal, registry and parent values match the PROOF lines below (one line per LEI found, with the registeredAs filter total and LEIs, the GLEIF fields used, and the parent LEI and legal name or the exception category and reason, verbatim).
4. The lapsed list (13), disagreement list (0), parent list (0 whose parent is another registrant of the 100; 0 with any direct parent LEI) and no-LEI list (10) below agree with gleif-400-pull3.csv.
5. The platform record shows PULL 1 (2026-11-18 04:02:44+00), PULL 2 (2026-11-19 04:20:40+00, 24.3 hours later) and PULL 3 (2026-11-20 04:27:57+00, 24.1 hours later), each with its CSV row count and SHA-256 as under DATA FILES; each pull source time (HTTP Date header of its first request) is later than the previous pull's (pull 1: 2026-11-18, pull 2: Thu, 19 Nov 2026 04:09:36 GMT, pull 3: Fri, 20 Nov 2026 04:21:19 GMT); the change counts below agree with the CSV files.

## Lists from pull 3 (gleif-400-pull3.csv)

### Found-by tally
- sec lei: 0
- legal name: 89
- former name: 1
- fuzzy: 0
- none: 10
- total: 100

### Lapsed (13)
- 0000783325 | WEC ENERGY GROUP, INC. | lei=549300Z7J9Q8KKCN0H32 | status=DUPLICATE | next_renewal=2016-06-16T09:45:00Z
- 0001051470 | CROWN CASTLE INC. | lei=8945004LYZ2UDJOX9U15 | status=LAPSED | next_renewal=2020-11-21T09:08:35Z
- 0001138118 | CBRE GROUP, INC. | lei=52990016II9MJ2OSWA10 | status=LAPSED | next_renewal=2019-12-17T14:42:43Z
- 0001628171 | Revolution Medicines, Inc. | lei=549300JU3X0LBCQ65892 | status=LAPSED | next_renewal=2021-12-11T10:56:00Z
- 0000878927 | OLD DOMINION FREIGHT LINE, INC. | lei=5299009TWK32WE417T96 | status=LAPSED | next_renewal=2019-11-23T08:00:27Z
- 0000839923 | VODAFONE GROUP PUBLIC LTD CO | lei=549300MSQV80HSATBG53 | status=DUPLICATE | next_renewal=2015-02-13T11:00:00Z
- 0001289490 | Extra Space Storage Inc. | lei=529900SDJHKRQWED6A16 | status=LAPSED | next_renewal=2020-03-04T10:30:38Z
- 0001027664 | ELBIT SYSTEMS LTD | lei=529900Q9CB1REUMZSS32 | status=LAPSED | next_renewal=2019-11-02T08:08:20Z
- 0001957132 | SharkNinja, Inc. | lei=549300UKI1IKQ5VX0403 | status=LAPSED | next_renewal=2026-02-09T09:14:42Z
- 0001172724 | GOLD FIELDS LTD | lei=5299003KXIBJQYCBBD72 | status=LAPSED | next_renewal=2020-09-12T08:07:38Z
- 0001406234 | Brookfield Infrastructure Partners L.P. | lei=549300WEH5R2OODI7Y90 | status=LAPSED | next_renewal=2017-06-13T13:03:00Z
- 0000920148 | LABCORP HOLDINGS INC. | lei=549300CDU4WF6Q2YMS76 | status=DUPLICATE | next_renewal=2014-06-05T17:16:00Z
- 0000719955 | WILLIAMS SONOMA INC | lei=549300IARG6YWVTZ1I92 | status=LAPSED | next_renewal=2014-03-27T17:59:00Z

### SEC lei vs name-search disagreements (0)
(none)

### Parent is another registrant of the 100 (0)
(none)

### Registrants with a direct parent LEI (0)
(none)

### No LEI (10)
- 0001805284 | Rocket Companies, Inc. | sec_lei=(none)
- 0002018139 | Toyota Tsusho Corporation/ADR | sec_lei=(none)
- 0001132924 | CHUNGHWA TELECOM CO LTD | sec_lei=(none)
- 0001033767 | UNITED MICROELECTRONICS CORP | sec_lei=(none)
- 0001070304 | ORIX CORP | sec_lei=(none)
- 0001973266 | TKO Group Holdings, Inc. | sec_lei=(none)
- 0000717826 | ERICSSON LM TELEPHONE CO | sec_lei=(none)
- 0001469059 | Capitec Limited/ADR | sec_lei=(none)
- 0001447391 | RESONA HOLDINGS INC | sec_lei=(none)
- 0001263043 | SHINHAN FINANCIAL GROUP CO LTD | sec_lei=(none)

## Changes

### PULL 2 vs PULL 1
New 0, gone 0, changed 24 cells; pull 1 rows 100, pull 2 rows 100 (later = earlier + new - gone).
- 0001650372 | name search lei | earlier: 5493005ANNO41NYIM267 | later: 549300V7ZY5P02D2MY38
- 0001650372 | lei | earlier: 5493005ANNO41NYIM267 | later: 549300V7ZY5P02D2MY38
- 0001650372 | found by | earlier: fuzzy | later: legal name
- 0001650372 | next_renewal | earlier: 2027-10-24T00:00:00Z | later: 2027-02-24T00:00:00Z
- 0001650372 | registeredAs | earlier: 102 443 916 | later: 6892214
- 0002041610 | found by | earlier: fuzzy | later: legal name
- 0001315098 | found by | earlier: fuzzy | later: legal name
- 0000839923 | found by | earlier: former name | later: legal name
- 0001167379 | found by | earlier: fuzzy | later: legal name
- 0000007084 | found by | earlier: fuzzy | later: legal name
- 0000073124 | name search lei | earlier: 549300U68JXSOE16IN60 | later: 549300GLF98S992BC502
- 0000073124 | lei | earlier: 549300U68JXSOE16IN60 | later: 549300GLF98S992BC502
- 0000073124 | found by | earlier: fuzzy | later: legal name
- 0000073124 | next_renewal | earlier: 2027-10-03T00:00:00Z | later: 2027-04-23T10:28:00Z
- 0000073124 | registeredAs | earlier:  | later: 774471
- 0000073124 | registry_unique | earlier:  | later: no
- 0001172724 | registry_unique | earlier: yes | later: 
- 0001116578 | name search lei | earlier: 213800ZQ434ONXTSFW67 | later: 5493001Z3ZE83NGK8Y12
- 0001116578 | lei | earlier: 213800ZQ434ONXTSFW67 | later: 5493001Z3ZE83NGK8Y12
- 0001116578 | found by | earlier: fuzzy | later: legal name
- 0001116578 | registration_status | earlier: RETIRED | later: ISSUED
- 0001116578 | next_renewal | earlier: 2025-06-22T00:00:00Z | later: 2027-01-08T00:18:00Z
- 0001116578 | lapsed | earlier: yes | later: no
- 0001116578 | registeredAs | earlier: O00008174_00000001 | later: 01397169

Note on the pull 2 changes: 24 changed cells across 7 CIKs. 3 LEIs corrected: pull 1 first pass matched them via fuzzy; pull 2 applied the rev2 ladder (raw->expanded->core) to all rows, so the legalName filter found the right record: 0001650372 Atlassian, 0000073124 Northern Trust, 0001116578 Prudential (RETIRED -> ISSUED, lapsed yes->no). 5 found-by upgrades with the same LEI (fuzzy->legal name: 0002041610 Skydance, 0001315098 Roblox, 0001167379 Alcon, 0000007084 ADM; former name->legal name: 0000839923 Vodafone). 1 stale value corrected: 0001172724 Gold Fields registry_unique yes->blank.

### PULL 3 vs PULL 2
no change: new 0, gone 0, changed 0 cells; pull 2 rows 100, pull 3 rows 100 (later = earlier + new - gone).

## PROOF

### Pull 3 source time and requests
Pull 3 source time (Date header of first request): Fri, 20 Nov 2026 04:21:19 GMT. Pull date (UTC): 2026-11-20. First request: 2026-11-20T04:21:18.181Z GET https://www.sec.gov/files/company_tickers.json -> 200 company_tickers.json (pull 3): ok
The full pull 3 request log (568 requests) cannot fit this Report under 150,000 characters together with the one-per-line PROOF lists, so requests are given as counts per endpoint:
- 191 x GET api.gleif.org/api/v1/lei-records?filter[entity.legalName]=<name>&page[size]=5&page[number]=<n>
- 100 x GET data.sec.gov/submissions/CIK##########.json
- 90 x GET api.gleif.org/api/v1/lei-records/<LEI>/direct-parent
- 90 x GET api.gleif.org/api/v1/lei-records/<LEI>/direct-parent-reporting-exception
- 87 x GET api.gleif.org/api/v1/lei-records?filter[entity.registeredAs]=<value>&page[size]=5
- 9 x GET api.gleif.org/api/v1/fuzzycompletions?field=entity.legalName&q=<first word>
- 1 x GET www.sec.gov/files/company_tickers.json
- total: 568 requests, 0 failed after one retry (FAILED SOURCES section below).

### Pull 1 and pull 2 first requests (other pulls: the first and any failed)
Pull 1: first Date header Wed, 18 Nov 2026 03:39:54 GMT; 0 failed sources. Pull 2: first Date header Thu, 19 Nov 2026 04:09:36 GMT; 0 failed sources. Full pull 1 and pull 2 proof files are kept with their CSVs (pull1-proof.txt, pull2-proof.txt).

### Pull 3 PROOF lists (verbatim from pull3-proof.txt)

```
NO-LEI REGISTRANTS — names each search returned (verbatim):
0001805284 | SEC name: Rocket Companies, Inc. | SEC lei: (none)
  0001805284 | legalName="Rocket Companies, Inc." (total 77542) -> ["INC Group Inc.", "INC", "Gazelle.ia Inc. / Gazelle.ai Inc.", "Pruvations Inc 401K Inc", "GIIG, Inc. TOOT, Inc.", "AVIYA INC.", "DVERACITY INC", "KoreLogic, Inc.", "PARLAYX INC.", "PINNGOODS INC.", "NANOPTIX INC", "EKLECMATIC INC.", "FACETEC INC", "Abria, Inc.", "Yotpo, Inc.", "SPREADMASTERS, INC.", "AIXENO INC", "DATANIMBUS, INC.", "CYMPHONY, INC.", "VANTOR INC.", "GLOBALEMOJIS INC", "PROBIOSPHERE INC.", "ADDIGY, INC.", "Inspiraholding Inc", "Veradek Inc.", "JMMOY, INC.", "Alphia Inc", "Limrun, Inc.", "HYPERCURRENT, INC.", "FIXION INC.", "ZAMBOLAN, INC.", "AMOS Inc.", "JOBEC, INC.", "MOXO, INC.", "Kiokii Inc.", "Embend, Inc.", "GRIDSIGHT, INC.", "ISOLAVERION INC.", "GLOBAL INC", "RIMBLE, INC.", "KHCDII, Inc.", "ATMOSPHERE INC", "EngFlow Inc.", "Aerospike, Inc.", "PR INC", "Guillotine Inc.", "VOTR INC.", "Derivnex Inc.", "ABACUS.AI, INC.", "SKILLEX INC."]
  0001805284 | legalName="Rocket Companies Incorporated" (total 0) -> []
  0001805284 | legalName="Rocket Companies" (total 0) -> []
  0001805284 | fuzzy q="Rocket" (total n/a) -> ["ROC ETF", "Rocet AB", "ROCKET IT", "ROCKEX AS", "Rockest OÜ", "Rockestate", "ROCKET ApS", "ROCKET MAN", "Rockton AB", "RONCKET IO"]
0002018139 | SEC name: Toyota Tsusho Corporation/ADR | SEC lei: (none)
  0002018139 | legalName="Toyota Tsusho Corporation" (total 0) -> []
  0002018139 | legalName="Toyota Tsusho" (total 32) -> ["TOYOTA TSUSHO EUROPE", "TOYOTA TSUSHO (SI) LTD", "TOYOTA TSUSHO CANADA INC.", "TOYOTA TSUSHO U.K. LIMITED", "TOYOTA TSUSHO METALS LIMITED", "Toyota Tsusho Wheatland Inc.", "TOYOTA TSUSHO AMERICA, INC.", "Toyota Tsusho (South Sea) Limited", "TOYOTA TSUSHO (AUSTRALASIA) PTY. LIMITED", "Toyota Tsusho Systems Europe GmbH", "Toyota Tsusho Petroleum Pte. Ltd.", "TOYOTA TSUSHO INDIA PRIVATE LIMITED", "Toyota Tsusho Systems US, Inc.", "Toyota Tsusho Systems Europe GmbH", "TOYOTA TSUSHO SUGAR TRADING LIMITED", "C.I. TOYOTA TSUSHO DE COLOMBIA S.A.S.", "TOYOTA TSUSHO BHARAT MOTOR PRIVATE LIMITED", "TOYOTA TSUSHO BHARAT AUTO PRIVATE LIMITED", "TOYOTA TSUSHO NEXTY ELECTRONICS EUROPE GmbH", "TOYOTA TSUSHO SYSTEMS INDIA PRIVATE LIMITED", "Toyota Tsusho Asia Pacific Pte. Ltd.", "TOYOTA TSUSHO AUTOMOBILE SOUTH LONDON LIMITED", "TOYOTA TSUSHO AUTOMOBILE LONDON HOLDINGS LIMITED", "Toyota Tsusho Europe S.A. Magyarországi Fióktelep", "BHARAT TOYOTA TSUSHO KIRLOSKAR MOTOR PRIVATE LIMITED", "TVS TOYOTA TSUSHO SUPPLY CHAIN SOLUTIONS LIMITED", "Toyota Tsusho South Pacific Holdings Pty Ltd", "TOYOTA TSUSHO INSURANCE BROKER INDIA PRIVATE LIMITED", "TOYOTA TSUSHO NEXTY ELECTRONICS INDIA PRIVATE LIMITED", "Toyota Tsusho Europe SA Czech Republic Branch", "TOYOTA TSUSHO NEXTY ELECTRONICS EUROPE GMBH SUCURSAL EN ESPAÑA", "TOYOTA TSUSHO NEXTY ELECTRONICS EUROPE GmbH Czech Republic Branch"]
  0002018139 | fuzzy q="Toyota" (total n/a) -> ["Tonotaco OÜ", "Toyota Trust", "Toy Tales LLP", "Toyota-Fonden", "Toyota Belgium", "TOYOTA CHILE S A", "TOYOTA-ASTRA MOTOR", "TOYOTA ROMANIA SRL", "TOYOTA CITY, S.L.U.", "TOYOTA MOTOR EUROPE"]
0001132924 | SEC name: CHUNGHWA TELECOM CO LTD | SEC lei: (none)
  0001132924 | legalName="CHUNGHWA TELECOM CO LTD" (total 0) -> []
  0001132924 | legalName="CHUNGHWA TELECOM Company Limited" (total 0) -> []
  0001132924 | legalName="CHUNGHWA TELECOM" (total 0) -> []
  0001132924 | fuzzy q="CHUNGHWA" (total n/a) -> ["CHUNGHWA PICTURE TUBES, LTD.", "CHUNG WAH STORE COMPANY LIMITED"]
0001033767 | SEC name: UNITED MICROELECTRONICS CORP | SEC lei: (none)
  0001033767 | legalName="UNITED MICROELECTRONICS CORP" (total 1) -> ["United Microelectronics Corp. ADRhedged(TM)"]
  0001033767 | legalName="UNITED MICROELECTRONICS Corporation" (total 0) -> []
  0001033767 | legalName="UNITED MICROELECTRONICS" (total 1) -> ["United Microelectronics Corp. ADRhedged(TM)"]
  0001033767 | fuzzy q="UNITED" (total n/a) -> ["UNITED", "UNITE", "Unite", "Unit-D", "UNITEA", "UNITER", "UNITECH", "UNITED.B", "UNITEE AS", "UNITEL AS"]
0001070304 | SEC name: ORIX CORP | SEC lei: (none)
  0001070304 | legalName="ORIX CORP" (total 0) -> []
  0001070304 | legalName="ORIX Corporation" (total 5) -> ["ORIX CORPORATION USA", "ORIX CORPORATION UK LIMITED", "ORIX AUSTRALIA CORPORATION LIMITED", "ORIX CORPORATION INDIA LIMITED", "ORIX CORPORATION EUROPE N.V."]
  0001070304 | legalName="ORIX" (total 27) -> ["Orix Aktiebolag", "ORIX MODARABA", "Orix Wealth Ltd.", "ORIX ADVISERS, LLC", "RECREATIVOS ORIX SL", "ORIX ENTERPRISES LTD", "ORIX REINSURANCE LIMITED", "ORIX CORPORATION USA", "ORIX CORPORATION UK LIMITED", "ORIX PACKAGING PRIVATE LIMITED", "ORIX NEW ZEALAND LIMITED", "ORIX AUSTRALIA CORPORATION LIMITED", "ORIX ASIA CAPITAL LIMITED", "BLACK ORIX PLUS, S.L.", "ORIX AVIATION SYSTEMS LIMITED", "ORIX CORPORATION INDIA LIMITED", "PT ORIX Indonesia Finance", "ORIX CORPORATION EUROPE N.V.", "ORIX PUBLIC FINANCE, LLC", "ORIX CORPORATE CAPITAL INC.", "ORIX CAPITAL MARKETS, LLC", "SNL ORIX FORT HAMILTON, LLC", "Sequoia Orix Investments III Ltd", "SNL ORIX THIRD AVE, LLC", "SNL ORIX BOSTON ROAD, LLC", "ORIX SERVICES PAKISTAN (PVT.) LIMITED", "ORIX LEASING & FINANCIAL SERVICES INDIA LIMITED"]
  0001070304 | fuzzy q="ORIX" (total n/a) -> ["OMIX", "Onix", "ORIA", "ORIM", "ORIS", "ORYX", "OSIX", "ORBIX", "ORIAL", "ORIAN"]
0001973266 | SEC name: TKO Group Holdings, Inc. | SEC lei: (none)
  0001973266 | legalName="TKO Group Holdings, Inc." (total 77542) -> ["INC Group Inc.", "INC", "Gazelle.ia Inc. / Gazelle.ai Inc.", "Pruvations Inc 401K Inc", "GIIG, Inc. TOOT, Inc.", "AVIYA INC.", "DVERACITY INC", "KoreLogic, Inc.", "PARLAYX INC.", "PINNGOODS INC.", "NANOPTIX INC", "EKLECMATIC INC.", "FACETEC INC", "Abria, Inc.", "Yotpo, Inc.", "SPREADMASTERS, INC.", "AIXENO INC", "DATANIMBUS, INC.", "CYMPHONY, INC.", "VANTOR INC.", "GLOBALEMOJIS INC", "PROBIOSPHERE INC.", "ADDIGY, INC.", "Inspiraholding Inc", "Veradek Inc.", "JMMOY, INC.", "Alphia Inc", "Limrun, Inc.", "HYPERCURRENT, INC.", "FIXION INC.", "ZAMBOLAN, INC.", "AMOS Inc.", "JOBEC, INC.", "MOXO, INC.", "Kiokii Inc.", "Embend, Inc.", "GRIDSIGHT, INC.", "ISOLAVERION INC.", "GLOBAL INC", "RIMBLE, INC.", "KHCDII, Inc.", "ATMOSPHERE INC", "EngFlow Inc.", "Aerospike, Inc.", "PR INC", "Guillotine Inc.", "VOTR INC.", "Derivnex Inc.", "ABACUS.AI, INC.", "SKILLEX INC."]
  0001973266 | legalName="TKO Group Holdings Incorporated" (total 0) -> []
  0001973266 | legalName="TKO Group Holdings" (total 0) -> []
  0001973266 | legalName="New Whale Inc." (former name "New Whale Inc.") (total 0) -> []
  0001973266 | legalName="New Whale Incorporated" (former name "New Whale Inc.") (total 0) -> []
  0001973266 | legalName="New Whale" (former name "New Whale Inc.") (total 0) -> []
  0001973266 | fuzzy q="TKO" (total n/a) -> ["TK", "TO", "TAO", "TKA", "TKG", "TKS", "TKW", "TMO", "TOM", "TOP"]
0000717826 | SEC name: ERICSSON LM TELEPHONE CO | SEC lei: (none)
  0000717826 | legalName="ERICSSON LM TELEPHONE CO" (total 0) -> []
  0000717826 | legalName="ERICSSON LM TELEPHONE Company" (total 0) -> []
  0000717826 | legalName="ERICSSON LM TELEPHONE" (total 0) -> []
  0000717826 | fuzzy q="ERICSSON" (total n/a) -> ["Ericsson AB", "ERICSSON AG", "ERICSSON AS", "Erickson B.V.", "ERICSSON GMBH", "Ericsson Inc.", "ERICSON, KJELL", "Eriksson Fur Ab", "ERICSSON LIMITED", "Ericsson Limited"]
0001469059 | SEC name: Capitec Limited/ADR | SEC lei: (none) | reverted to none: ladder matched "CAPITEC PTY LTD" (AU), a different entity from the registrant Capitec Bank Holdings Ltd (South Africa) — same judgment as pull 1 rev2; no name-equal GLEIF record exists ("Capitec Bank Holdings Limited" -> 0 results; "Capitec Limited" -> only "Capitec Bank Limited", a subsidiary)
  0001469059 | legalName="Capitec Limited" (total 1) -> ["Capitec Bank Limited"]
  0001469059 | legalName="Capitec" (total 2) -> ["CAPITEC PTY LTD", "Capitec Bank Limited"]
0001447391 | SEC name: RESONA HOLDINGS INC | SEC lei: (none)
  0001447391 | legalName="RESONA HOLDINGS INC" (total 0) -> []
  0001447391 | legalName="RESONA HOLDINGS Incorporated" (total 0) -> []
  0001447391 | legalName="RESONA HOLDINGS" (total 0) -> []
  0001447391 | fuzzy q="RESONA" (total n/a) -> ["Renona", "RESO AS", "RESONEO", "Reson Oy", "RESONANS", "RESONILO", "Recona AB", "RESONANCE", "RESOSA SL", "Reconar SA"]
0001263043 | SEC name: SHINHAN FINANCIAL GROUP CO LTD | SEC lei: (none)
  0001263043 | legalName="SHINHAN FINANCIAL GROUP CO LTD" (total 0) -> []
  0001263043 | legalName="SHINHAN FINANCIAL GROUP Company Limited" (total 0) -> []
  0001263043 | legalName="SHINHAN FINANCIAL GROUP" (total 0) -> []
  0001263043 | fuzzy q="SHINHAN" (total n/a) -> ["Shinano Fund", "Shinkansen Oy", "SHIHAN OVERSEAS", "SHISHANT AGARWAL", "SHISHAN KUMAR GARG", "Shinhan Bank Canada", "Shinhan Asia Limited", "Shinhan Bank America", "SHINHAN BANK CO., LTD", "SHINHAN BANK EUROPE GmbH"]

LEI DETAILS — one line each (registeredAs filter total and LEIs, GLEIF fields used, parent LEI and legal name or exception category and reason, verbatim):
0000097210 | lei=C3X4YJ278QNZHRJULN75 | found by=legal name | matched GLEIF name="TERADYNE, INC." | status=ISSUED | nextRenewal=2027-07-24T17:05:07Z | registeredAs=042272148 | registeredAs filter total=1 LEIs=[C3X4YJ278QNZHRJULN75] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0000097210 | legalName="TERADYNE, INC" (total 77550) -> ["TERADYNE, INC.", "TERADYNE", "TERADYNE LIMITED", "TERADYNE ITALIA SRL", "TERADYNE (ASIA) PTE. LTD."]
0002073893 | lei=5493002GJ0NJP1HI0C79 | found by=legal name | matched GLEIF name="DOLLARAMA INC." | status=ISSUED | nextRenewal=2027-11-20T16:19:30Z | registeredAs=453739-4 | registeredAs filter total=1 LEIs=[5493002GJ0NJP1HI0C79] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0002073893 | legalName="Dollarama Inc." (total 1) -> ["DOLLARAMA INC."]
0001754301 | lei=549300DDU6FDRBIELS05 | found by=legal name | matched GLEIF name="FOX CORPORATION" | status=ISSUED | nextRenewal=2027-09-14T14:43:11Z | registeredAs=6866021 | registeredAs filter total=1 LEIs=[549300DDU6FDRBIELS05] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0001754301 | legalName="Fox Corp" (total 6) -> ["SILVER FOX CORP.", "ARCTIC FOX LITHIUM CORP.", "Running Fox Resource Corp.", "FOX FACTORY HOLDING CORP.", "FOX INTERNATIONAL GROUP CORP.", "Grey Fox Holdings Corp."]
  0001754301 | legalName="Fox Corporation" (total 6) -> ["FOX CORPORATION", "Cape Fox Corporation", "Fox Products Corporation", "RED FOX CD ACQUISITION CORPORATION", "Fox Hill Village Homeowners Corporation"]
0000783325 | lei=549300Z7J9Q8KKCN0H32 | found by=legal name | matched GLEIF name="WEC Energy Group Inc." | status=DUPLICATE | nextRenewal=2016-06-16T09:45:00Z | registeredAs= | registeredAs filter total=null LEIs=[] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=none
  0000783325 | legalName="WEC ENERGY GROUP, INC." (total 77542) -> ["WEC Energy Group Inc.", "WEC ENERGY GROUP INC.", "INC Group Inc.", "INC", "Gazelle.ia Inc. / Gazelle.ai Inc."]
0001736297 | lei=529900LJL8TUEGF7HG20 | found by=legal name | matched GLEIF name="ASTERA LABS, INC." | status=ISSUED | nextRenewal=2027-09-26T14:25:28Z | registeredAs=6593628 | registeredAs filter total=1 LEIs=[529900LJL8TUEGF7HG20] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001736297 | legalName="Astera Labs, Inc." (total 77542) -> ["ASTERA LABS, INC.", "INC Group Inc.", "INC", "Gazelle.ia Inc. / Gazelle.ai Inc.", "Pruvations Inc 401K Inc"]
0001051470 | lei=8945004LYZ2UDJOX9U15 | found by=legal name | matched GLEIF name="Crown Castle Inc" | status=LAPSED | nextRenewal=2020-11-21T09:08:35Z | registeredAs=980212790 | registeredAs filter total=1 LEIs=[8945004LYZ2UDJOX9U15] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001051470 | legalName="CROWN CASTLE INC." (total 2) -> ["Crown Castle Inc", "CROWN CASTLE INC."]
0001035983 | lei=5299009DT1ZA5HTU6R38 | found by=legal name | matched GLEIF name="COMFORT SYSTEMS USA, INC." | status=ISSUED | nextRenewal=2027-05-08T16:01:25Z | registeredAs=2693796 | registeredAs filter total=1 LEIs=[5299009DT1ZA5HTU6R38] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001035983 | legalName="COMFORT SYSTEMS USA INC" (total 1) -> ["COMFORT SYSTEMS USA, INC."]
0001138118 | lei=52990016II9MJ2OSWA10 | found by=legal name | matched GLEIF name="CBRE Group, Inc." | status=LAPSED | nextRenewal=2019-12-17T14:42:43Z | registeredAs=5033789 | registeredAs filter total=1 LEIs=[52990016II9MJ2OSWA10] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0001138118 | legalName="CBRE GROUP, INC." (total 77542) -> ["CBRE Group, Inc.", "INC Group Inc.", "INC", "Gazelle.ia Inc. / Gazelle.ai Inc.", "Pruvations Inc 401K Inc"]
0001650372 | lei=549300V7ZY5P02D2MY38 | found by=legal name | matched GLEIF name="ATLASSIAN CORPORATION" | status=ISSUED | nextRenewal=2027-02-24T00:00:00Z | registeredAs=6892214 | registeredAs filter total=1 LEIs=[549300V7ZY5P02D2MY38] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0001650372 | legalName="Atlassian Corp" (total 0) -> []
  0001650372 | legalName="Atlassian Corporation" (total 2) -> ["ATLASSIAN CORPORATION", "ATLASSIAN CORPORATION PLC"]
0002041610 | lei=549300XA8RHE8K25T170 | found by=legal name | matched GLEIF name="SKYDANCE LTD." | status=ISSUED | nextRenewal=2026-12-29T09:11:00Z | registeredAs=OI-311842 | registeredAs filter total=1 LEIs=[549300XA8RHE8K25T170] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0002041610 | legalName="Skydance Corp" (total 0) -> []
  0002041610 | legalName="Skydance Corporation" (total 1) -> ["PARAMOUNT SKYDANCE CORPORATION"]
  0002041610 | legalName="Skydance" (total 4) -> ["SKYDANCE LTD.", "PARAMOUNT SKYDANCE CORPORATION", "Skydance Capital Ltd.", "SKYDANCE PRODUCTIONS, LLC"]
0000096021 | lei=5RGWIFLMGH3YS7KWI652 | found by=legal name | matched GLEIF name="SYSCO CORPORATION" | status=ISSUED | nextRenewal=2027-12-01T16:45:15Z | registeredAs=712404 | registeredAs filter total=1 LEIs=[5RGWIFLMGH3YS7KWI652] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0000096021 | legalName="SYSCO CORP" (total 0) -> []
  0000096021 | legalName="SYSCO Corporation" (total 3) -> ["SYSCO CORPORATION", "SYSCO HOLDINGS CORPORATION", "SYSCO CORPORATION RETIREMENT PLAN"]
0001471055 | lei=549300D1H731B30TSI43 | found by=legal name | matched GLEIF name="BANCO SANTANDER (BRASIL) S.A." | status=ISSUED | nextRenewal=2027-10-10T18:01:00Z | registeredAs=90.400.888/0001-42 | registeredAs filter total=2 LEIs=[894500TRC74NXKWXOS50, 549300D1H731B30TSI43] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_PUBLIC
  0001471055 | legalName="Banco Santander (Brasil) S.A." (total 1) -> ["BANCO SANTANDER (BRASIL) S.A."]
0000788784 | lei=PUSS41EMO3E6XXNV3U28 | found by=legal name | matched GLEIF name="PUBLIC SERVICE ENTERPRISE GROUP INCORPORATED" | status=ISSUED | nextRenewal=2027-07-15T18:20:48Z | registeredAs=0100267099 | registeredAs filter total=1 LEIs=[PUSS41EMO3E6XXNV3U28] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0000788784 | legalName="PUBLIC SERVICE ENTERPRISE GROUP INC" (total 0) -> []
  0000788784 | legalName="PUBLIC SERVICE ENTERPRISE GROUP Incorporated" (total 3) -> ["PUBLIC SERVICE ENTERPRISE GROUP INCORPORATED", "Public Service Enterprise Group Incorporated Master Retirement Trust", "Public Service Enterprise Group Incorporated Master Defined Benefit Retirement Trust"]
0001549802 | lei=549300HVTWB0GJZ16V92 | found by=legal name | matched GLEIF name="JD.com, Inc." | status=ISSUED | nextRenewal=2027-03-04T14:52:00Z | registeredAs=284373 | registeredAs filter total=1 LEIs=[549300HVTWB0GJZ16V92] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NATURAL_PERSONS
  0001549802 | legalName="JD.com, Inc." (total 77546) -> ["JD.com, Inc.", "JD.com International Limited", "JD.COM INTERNATIONAL (SINGAPORE) PTE. LIMITED", "JD.COM ASIA PACIFIC INVESTMENT LIMITED", "JD.com E-commerce (Investment) Hong Kong Corporation Limited"]
0001932393 | lei=549300OI9J7XOWZMUN85 | found by=legal name | matched GLEIF name="GE HEALTHCARE TECHNOLOGIES INC." | status=ISSUED | nextRenewal=2027-10-20T15:08:49Z | registeredAs=6772877 | registeredAs filter total=1 LEIs=[549300OI9J7XOWZMUN85] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0001932393 | legalName="GE HealthCare Technologies Inc." (total 1) -> ["GE HEALTHCARE TECHNOLOGIES INC."]
0001628171 | lei=549300JU3X0LBCQ65892 | found by=legal name | matched GLEIF name="REVOLUTION MEDICINES, INC." | status=LAPSED | nextRenewal=2021-12-11T10:56:00Z | registeredAs=5611600 | registeredAs filter total=1 LEIs=[549300JU3X0LBCQ65892] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_PUBLIC
  0001628171 | legalName="Revolution Medicines, Inc." (total 77542) -> ["REVOLUTION MEDICINES, INC.", "INC Group Inc.", "INC", "Gazelle.ia Inc. / Gazelle.ai Inc.", "Pruvations Inc 401K Inc"]
0000875045 | lei=W8J5WZB5IY3K0NDQT671 | found by=legal name | matched GLEIF name="BIOGEN INC." | status=ISSUED | nextRenewal=2027-02-19T21:48:17Z | registeredAs=2726078 | registeredAs filter total=2 LEIs=[W8J5WZB5IY3K0NDQT671, 74370068B64Z2A5G8588] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0000875045 | legalName="BIOGEN INC." (total 2) -> ["BIOGEN INC.", "BIOGEN MA INC."]
0000874766 | lei=IU7C3FTM7Y3BQM112U94 | found by=legal name | matched GLEIF name="THE HARTFORD INSURANCE GROUP, INC." | status=ISSUED | nextRenewal=2027-07-11T12:19:07Z | registeredAs=2077692 | registeredAs filter total=1 LEIs=[IU7C3FTM7Y3BQM112U94] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0000874766 | legalName="HARTFORD INSURANCE GROUP, INC." (total 77542) -> ["THE HARTFORD INSURANCE GROUP, INC.", "INC Group Inc.", "INC", "Gazelle.ia Inc. / Gazelle.ai Inc.", "Pruvations Inc 401K Inc"]
0000916076 | lei=5299005MZ4WZECVATV08 | found by=legal name | matched GLEIF name="Martin Marietta Materials, Inc." | status=ISSUED | nextRenewal=2027-02-19T09:44:48Z | registeredAs=0333756 | registeredAs filter total=1 LEIs=[5299005MZ4WZECVATV08] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0000916076 | legalName="MARTIN MARIETTA MATERIALS INC" (total 2) -> ["Martin Marietta Materials, Inc.", "Martin Marietta Materials, Inc. Defined Benefit Plans Master Retirement Trust"]
0000100517 | lei=98450079DA0B78DD6764 | found by=legal name | matched GLEIF name="UNITED AIRLINES HOLDINGS, INC." | status=ISSUED | nextRenewal=2027-08-20T08:33:51Z | registeredAs=697326 | registeredAs filter total=1 LEIs=[98450079DA0B78DD6764] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NATURAL_PERSONS
  0000100517 | legalName="United Airlines Holdings, Inc." (total 77542) -> ["UNITED AIRLINES HOLDINGS, INC.", "INC Group Inc.", "INC", "Gazelle.ia Inc. / Gazelle.ai Inc.", "Pruvations Inc 401K Inc"]
0001474432 | lei=549300NPDB0BZTK3WO90 | found by=legal name | matched GLEIF name="EVERPURE, INC." | status=ISSUED | nextRenewal=2027-08-20T00:00:00Z | registeredAs=4737699 | registeredAs filter total=1 LEIs=[549300NPDB0BZTK3WO90] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001474432 | legalName="Everpure, Inc." (total 77542) -> ["EVERPURE, INC.", "INC Group Inc.", "INC", "Gazelle.ia Inc. / Gazelle.ai Inc.", "Pruvations Inc 401K Inc"]
0000947484 | lei=549300AYR4P8AFKDCE43 | found by=legal name | matched GLEIF name="Arch Capital Group Ltd." | status=ISSUED | nextRenewal=2027-10-09T18:00:00Z | registeredAs=29407 | registeredAs filter total=3 LEIs=[549300AYR4P8AFKDCE43, 529900UPL8W2O69H1I13, 1595S7GHHG6LDH79K965] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0000947484 | legalName="ARCH CAPITAL GROUP LTD." (total 1) -> ["Arch Capital Group Ltd."]
0001396009 | lei=549300Q8LSNHAVWBNI21 | found by=legal name | matched GLEIF name="VULCAN MATERIALS COMPANY" | status=ISSUED | nextRenewal=2027-04-30T05:37:08Z | registeredAs=0100975660 | registeredAs filter total=1 LEIs=[549300Q8LSNHAVWBNI21] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0001396009 | legalName="Vulcan Materials CO" (total 0) -> []
  0001396009 | legalName="Vulcan Materials Company" (total 2) -> ["VULCAN MATERIALS COMPANY", "VULCAN MATERIALS COMPANY MASTER PENSION TRUST"]
0000878927 | lei=5299009TWK32WE417T96 | found by=legal name | matched GLEIF name="Old Dominion Freight Line, Inc." | status=LAPSED | nextRenewal=2019-11-23T08:00:27Z | registeredAs=3306981 | registeredAs filter total=1 LEIs=[5299009TWK32WE417T96] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0000878927 | legalName="OLD DOMINION FREIGHT LINE, INC." (total 77542) -> ["Old Dominion Freight Line, Inc.", "INC Group Inc.", "INC", "Gazelle.ia Inc. / Gazelle.ai Inc.", "Pruvations Inc 401K Inc"]
0001002047 | lei=QTX3D84DZDD5JYOCYH15 | found by=legal name | matched GLEIF name="NETAPP, INC." | status=ISSUED | nextRenewal=2027-01-31T20:50:52Z | registeredAs=3452743 | registeredAs filter total=1 LEIs=[QTX3D84DZDD5JYOCYH15] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NATURAL_PERSONS
  0001002047 | legalName="NetApp, Inc." (total 77557) -> ["NETAPP, INC.", "Netapp Belgium", "NetApp B.V.", "NETAPP SOUTH AFRICA", "NetApp Austria GmbH"]
0001315098 | lei=529900ANZDBDFU91SO19 | found by=legal name | matched GLEIF name="ROBLOX CORPORATION" | status=ISSUED | nextRenewal=2026-12-16T10:14:52Z | registeredAs=E49322182025-6 | registeredAs filter total=1 LEIs=[529900ANZDBDFU91SO19] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001315098 | legalName="Roblox Corp" (total 0) -> []
  0001315098 | legalName="Roblox Corporation" (total 1) -> ["ROBLOX CORPORATION"]
0000839923 | lei=549300MSQV80HSATBG53 | found by=legal name | matched GLEIF name="VODAFONE GROUP PUBLIC LIMITED COMPANY" | status=DUPLICATE | nextRenewal=2015-02-13T11:00:00Z | registeredAs=01833679 | registeredAs filter total=2 LEIs=[549300MSQV80HSATBG53, 213800TB53ELEUKM7Q61] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=none
  0000839923 | legalName="VODAFONE GROUP PUBLIC LTD CO" (total 0) -> []
  0000839923 | legalName="VODAFONE GROUP PUBLIC Limited Company" (total 2) -> ["VODAFONE GROUP PUBLIC LIMITED COMPANY", "VODAFONE GROUP PUBLIC LIMITED COMPANY"]
0001167379 | lei=9676001NFC8U0KVWE816 | found by=legal name | matched GLEIF name="ALCON" | status=ISSUED | nextRenewal=2026-12-07T03:20:40Z | registeredAs=0442.880.917 | registeredAs filter total=1 LEIs=[9676001NFC8U0KVWE816] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0001167379 | legalName="ALCON INC" (total 1) -> ["Alcon Industries, Inc."]
  0001167379 | legalName="ALCON Incorporated" (total 0) -> []
  0001167379 | legalName="ALCON" (total 49) -> ["ALCON", "ALCON DEVELOPERS", "ALCON AG", "Alcon GmbH", "ALCON S.R.L."]
0001071739 | lei=549300Z7JJ4TQSQGT333 | found by=legal name | matched GLEIF name="CENTENE CORPORATION" | status=ISSUED | nextRenewal=2027-03-24T16:29:17Z | registeredAs=3439838 | registeredAs filter total=1 LEIs=[549300Z7JJ4TQSQGT333] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001071739 | legalName="CENTENE CORP" (total 0) -> []
  0001071739 | legalName="CENTENE Corporation" (total 1) -> ["CENTENE CORPORATION"]
0000047111 | lei=21X2CX66SU2BR6QTAD08 | found by=legal name | matched GLEIF name="THE HERSHEY COMPANY" | status=ISSUED | nextRenewal=2027-01-24T20:29:42Z | registeredAs=224803 | registeredAs filter total=1 LEIs=[21X2CX66SU2BR6QTAD08] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0000047111 | legalName="HERSHEY CO" (total 1) -> ["HERSHEY EQUIPMENT CO., INC."]
  0000047111 | legalName="HERSHEY Company" (total 3) -> ["HERSHEY CREAMERY COMPANY", "THE HERSHEY COMPANY", "THE HERSHEY COMPANY MASTER RETIREMENT TRUST"]
0001890126 | lei=724500GJBUL3D9TW9Y18 | found by=legal name | matched GLEIF name="Universal Music Group N.V." | status=ISSUED | nextRenewal=2027-07-28T13:39:11Z | registeredAs=81106661 | registeredAs filter total=1 LEIs=[724500GJBUL3D9TW9Y18] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0001890126 | legalName="Universal Music Group N.V." (total 1) -> ["Universal Music Group N.V."]
0001618756 | lei=5299009RXTX9DN9AKJ98 | found by=legal name | matched GLEIF name="Restaurant Brands International Inc." | status=ISSUED | nextRenewal=2027-06-29T17:02:05Z | registeredAs=906066-9 | registeredAs filter total=1 LEIs=[5299009RXTX9DN9AKJ98] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0001618756 | legalName="Restaurant Brands International Inc." (total 1) -> ["Restaurant Brands International Inc."]
0001289490 | lei=529900SDJHKRQWED6A16 | found by=legal name | matched GLEIF name="EXTRA SPACE STORAGE" | status=LAPSED | nextRenewal=2020-03-04T10:30:38Z | registeredAs=10679291-0151 | registeredAs filter total=1 LEIs=[529900SDJHKRQWED6A16] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001289490 | legalName="Extra Space Storage Inc." (total 0) -> []
  0001289490 | legalName="Extra Space Storage Incorporated" (total 0) -> []
  0001289490 | legalName="Extra Space Storage" (total 2) -> ["EXTRA SPACE STORAGE", "EXTRA SPACE STORAGE LP"]
0000007084 | lei=549300LO13MQ9HYSTR83 | found by=legal name | matched GLEIF name="ARCHER-DANIELS-MIDLAND COMPANY" | status=ISSUED | nextRenewal=2027-10-03T18:01:00Z | registeredAs=152524 | registeredAs filter total=1 LEIs=[549300LO13MQ9HYSTR83] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0000007084 | legalName="Archer-Daniels-Midland Co" (total 0) -> []
  0000007084 | legalName="Archer Daniels Midland Company" (total 1) -> ["ARCHER-DANIELS-MIDLAND COMPANY"]
0001037646 | lei=5493000BD5GJNUDIUG10 | found by=legal name | matched GLEIF name="METTLER-TOLEDO INTERNATIONAL INC." | status=ISSUED | nextRenewal=2027-08-16T19:13:47Z | registeredAs=2281086 | registeredAs filter total=1 LEIs=[5493000BD5GJNUDIUG10] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NATURAL_PERSONS
  0001037646 | legalName="METTLER TOLEDO INTERNATIONAL INC/" (total 1) -> ["METTLER-TOLEDO INTERNATIONAL INC."]
0001555280 | lei=549300HD9Q1LOC9KLJ48 | found by=legal name | matched GLEIF name="ZOETIS INC." | status=ISSUED | nextRenewal=2027-07-11T11:34:24Z | registeredAs=5118663 | registeredAs filter total=1 LEIs=[549300HD9Q1LOC9KLJ48] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001555280 | legalName="Zoetis Inc." (total 2) -> ["ZOETIS INC.", "ZOETIS PHILIPPINES, INC."]
0001679788 | lei=5493004G3J2SC154DU06 | found by=legal name | matched GLEIF name="Coinbase Global, Inc." | status=ISSUED | nextRenewal=2027-04-21T13:10:29Z | registeredAs=0806346623 | registeredAs filter total=1 LEIs=[5493004G3J2SC154DU06] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0001679788 | legalName="Coinbase Global, Inc." (total 77542) -> ["Coinbase Global, Inc.", "INC Group Inc.", "INC", "Gazelle.ia Inc. / Gazelle.ai Inc.", "Pruvations Inc 401K Inc"]
0000798354 | lei=GI7UBEJLXYLGR2C7GV83 | found by=legal name | matched GLEIF name="FISERV, INC." | status=ISSUED | nextRenewal=2027-08-03T12:39:23Z | registeredAs=F024977 | registeredAs filter total=1 LEIs=[GI7UBEJLXYLGR2C7GV83] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0000798354 | legalName="FISERV INC" (total 1) -> ["FISERV, INC."]
0001725964 | lei=5493002QQ7GD21OWF963 | found by=legal name | matched GLEIF name="NUTRIEN LTD." | status=ISSUED | nextRenewal=2027-03-27T17:14:29Z | registeredAs=1026366-4 | registeredAs filter total=1 LEIs=[5493002QQ7GD21OWF963] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0001725964 | legalName="Nutrien Ltd." (total 2) -> ["NUTRIEN LTD.", "NUTRIEN AG SOLUTIONS FERTILISER PTY LTD"]
0000943819 | lei=529900T3QE5253CCXF22 | found by=legal name | matched GLEIF name="RESMED INC." | status=ISSUED | nextRenewal=2027-01-24T11:00:26Z | registeredAs=2390651 | registeredAs filter total=1 LEIs=[529900T3QE5253CCXF22] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0000943819 | legalName="RESMED INC" (total 1) -> ["RESMED INC."]
0001020569 | lei=SQL3F6CKNNBM3SQGHX24 | found by=legal name | matched GLEIF name="IRON MOUNTAIN INCORPORATED" | status=ISSUED | nextRenewal=2027-04-01T06:40:14Z | registeredAs=5559325 | registeredAs filter total=1 LEIs=[SQL3F6CKNNBM3SQGHX24] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001020569 | legalName="IRON MOUNTAIN INC" (total 1) -> ["IRON MOUNTAIN US HOLDINGS, INC."]
  0001020569 | legalName="IRON MOUNTAIN Incorporated" (total 1) -> ["IRON MOUNTAIN INCORPORATED"]
0002083785 | lei=529900W4BQDNMAOSRA49 | found by=legal name | matched GLEIF name="SUNBELT RENTALS HOLDINGS, INC." | status=ISSUED | nextRenewal=2027-10-17T07:18:04Z | registeredAs=10072303 | registeredAs filter total=1 LEIs=[529900W4BQDNMAOSRA49] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0002083785 | legalName="Sunbelt Rentals Holdings, Inc." (total 77542) -> ["SUNBELT RENTALS HOLDINGS, INC.", "INC Group Inc.", "INC", "Gazelle.ia Inc. / Gazelle.ai Inc.", "Pruvations Inc 401K Inc"]
0000904868 | lei=XDFJ0CYCOO1FXRFTQS51 | found by=legal name | matched GLEIF name="Fresenius SE & Co. KGaA" | status=ISSUED | nextRenewal=2027-11-28T16:01:17Z | registeredAs=HRB 11852 | registeredAs filter total=3 LEIs=[529900ME6QY0C5M7CY59, 529900EIVPE9J0RLF720, XDFJ0CYCOO1FXRFTQS51] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0000904868 | legalName="Fresenius SE & Co. KGaA" (total 1) -> ["Fresenius SE & Co. KGaA"]
0000827054 | lei=5493007PTFULNYZJ1R12 | found by=legal name | matched GLEIF name="MICROCHIP TECHNOLOGY INCORPORATED" | status=ISSUED | nextRenewal=2027-02-01T18:21:33Z | registeredAs=2187388 | registeredAs filter total=1 LEIs=[5493007PTFULNYZJ1R12] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0000827054 | legalName="MICROCHIP TECHNOLOGY INC" (total 0) -> []
  0000827054 | legalName="MICROCHIP TECHNOLOGY Incorporated" (total 1) -> ["MICROCHIP TECHNOLOGY INCORPORATED"]
0002007855 | lei=2549007XC91CAB3E0N98 | found by=legal name | matched GLEIF name="VENTURE GLOBAL, INC." | status=ISSUED | nextRenewal=2027-08-02T19:45:31Z | registeredAs=2378580 | registeredAs filter total=1 LEIs=[2549007XC91CAB3E0N98] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_PUBLIC
  0002007855 | legalName="Venture Global, Inc." (total 77549) -> ["VENTURE GLOBAL, INC.", "VENTURE GLOBAL LNG, INC.", "VENTURE GLOBAL COMMODITIES, LLC", "ORIENT VENTURE GLOBAL LIMITED", "Venture Global Shipping Holdings, LLC"]
0001027664 | lei=529900Q9CB1REUMZSS32 | found by=legal name | matched GLEIF name="Elbit Systems Ltd." | status=LAPSED | nextRenewal=2019-11-02T08:08:20Z | registeredAs=520043027 | registeredAs filter total=1 LEIs=[529900Q9CB1REUMZSS32] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0001027664 | legalName="ELBIT SYSTEMS LTD" (total 1) -> ["Elbit Systems Ltd."]
0000033213 | lei=4NT01YGM4X7ZX86ISY52 | found by=legal name | matched GLEIF name="EQT CORPORATION" | status=ISSUED | nextRenewal=2027-01-12T12:43:14Z | registeredAs=3816419 | registeredAs filter total=1 LEIs=[4NT01YGM4X7ZX86ISY52] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0000033213 | legalName="EQT Corp" (total 0) -> []
  0000033213 | legalName="EQT Corporation" (total 1) -> ["EQT CORPORATION"]
0001447669 | lei=5493004W8TRGD63APX93 | found by=legal name | matched GLEIF name="TWILIO INC." | status=ISSUED | nextRenewal=2027-03-08T16:38:26Z | registeredAs=4518652 | registeredAs filter total=1 LEIs=[5493004W8TRGD63APX93] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0001447669 | legalName="TWILIO INC" (total 1) -> ["TWILIO INC."]
0001022671 | lei=549300HGGKEL4FYTTQ83 | found by=legal name | matched GLEIF name="STEEL DYNAMICS, INC." | status=ISSUED | nextRenewal=2027-02-25T16:48:17Z | registeredAs=1994061014 | registeredAs filter total=1 LEIs=[549300HGGKEL4FYTTQ83] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NATURAL_PERSONS
  0001022671 | legalName="STEEL DYNAMICS INC" (total 1) -> ["STEEL DYNAMICS, INC."]
0001699150 | lei=5299004C02FMZCUOIR50 | found by=legal name | matched GLEIF name="INGERSOLL RAND INC." | status=ISSUED | nextRenewal=2027-05-14T16:31:39Z | registeredAs=5295941 | registeredAs filter total=2 LEIs=[5299004C02FMZCUOIR50, 549300UWX2Z43DLGB776] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0001699150 | legalName="Ingersoll Rand Inc." (total 3) -> ["INGERSOLL RAND INC.", "INGERSOLL-RAND INDUSTRIAL U.S., INC.", "Ingersoll-Rand Industrial US Inc Pension Trust"]
0000720005 | lei=RGUZHJ05YTITL6D76949 | found by=legal name | matched GLEIF name="RAYMOND JAMES FINANCIAL, INC." | status=ISSUED | nextRenewal=2027-01-05T11:16:55Z | registeredAs=444750 | registeredAs filter total=2 LEIs=[894500646MVMU4CA6K40, RGUZHJ05YTITL6D76949] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0000720005 | legalName="RAYMOND JAMES FINANCIAL INC" (total 4) -> ["RAYMOND JAMES FINANCIAL, INC.", "RAYMOND JAMES FINANCIAL SERVICES, INC.", "Raymond James Financial Products, Inc.", "RAYMOND JAMES FINANCIAL SERVICES ADVISORS, INC."]
0000073124 | lei=549300GLF98S992BC502 | found by=legal name | matched GLEIF name="NORTHERN TRUST CORPORATION" | status=ISSUED | nextRenewal=2027-04-23T10:28:00Z | registeredAs=774471 | registeredAs filter total=2 LEIs=[213800WP6AX8PULC3496, 549300GLF98S992BC502] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0000073124 | legalName="NORTHERN TRUST CORP" (total 0) -> []
  0000073124 | legalName="NORTHERN TRUST Corporation" (total 2) -> ["NORTHERN TRUST CORPORATION", "NORTHERN TRUST INTERNATIONAL BANKING CORPORATION, THE"]
0001660134 | lei=549300N8J06I8MRHU620 | found by=legal name | matched GLEIF name="OKTA, INC." | status=ISSUED | nextRenewal=2027-01-22T14:23:01Z | registeredAs=4794941 | registeredAs filter total=1 LEIs=[549300N8J06I8MRHU620] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001660134 | legalName="Okta, Inc." (total 77551) -> ["OKTA, INC.", "OKTA", "Okta-Group Oy", "OKTA RENEWABLES GMBH", "Okta Finance GmbH"]
0001957132 | lei=549300UKI1IKQ5VX0403 | found by=legal name | matched GLEIF name="SHARKNINJA PTY. LTD." | status=LAPSED | nextRenewal=2026-02-09T09:14:42Z | registeredAs=147 260 197 | registeredAs filter total=1 LEIs=[549300UKI1IKQ5VX0403] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001957132 | legalName="SharkNinja, Inc." (total 77546) -> ["SHARKNINJA EUROPE LTD", "SHARKNINJA OPERATING LLC", "SHARKNINJA PTY. LTD.", "SHARKNINJA APPLIANCE LLC", "INC Group Inc."]
0001513845 | lei=549300GGZHJ5Q1B18P93 | found by=legal name | matched GLEIF name="Nebius Group N.V." | status=ISSUED | nextRenewal=2027-02-28T03:23:00Z | registeredAs=27265167 | registeredAs filter total=1 LEIs=[549300GGZHJ5Q1B18P93] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0001513845 | legalName="Nebius Group N.V." (total 1) -> ["Nebius Group N.V."]
0000049196 | lei=549300XTVCVV9I7B5T19 | found by=legal name | matched GLEIF name="HUNTINGTON BANCSHARES INCORPORATED" | status=ISSUED | nextRenewal=2027-08-20T14:09:00Z | registeredAs=D00120733 | registeredAs filter total=1 LEIs=[549300XTVCVV9I7B5T19] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0000049196 | legalName="HUNTINGTON BANCSHARES INC" (total 0) -> []
  0000049196 | legalName="HUNTINGTON BANCSHARES Incorporated" (total 1) -> ["HUNTINGTON BANCSHARES INCORPORATED"]
0001172724 | lei=5299003KXIBJQYCBBD72 | found by=legal name | matched GLEIF name="Gold Fields Limited" | status=LAPSED | nextRenewal=2020-09-12T08:07:38Z | registeredAs= | registeredAs filter total=null LEIs=[] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001172724 | legalName="GOLD FIELDS LTD" (total 2) -> ["NORTON GOLD FIELDS PTY LTD", "GOLD FIELDS HOLDING PTY LTD"]
  0001172724 | legalName="GOLD FIELDS Limited" (total 5) -> ["Gold Fields Limited", "Gold Fields Ghana Limited", "GOLD FIELDS AUSTRALASIA (BVI) LIMITED", "GOLD FIELDS AUSTRALIA PTY LIMITED", "GOLD FIELDS OROGEN HOLDING (BVI) LIMITED"]
0001434265 | lei=529900MTJPDPE4MHJ122 | found by=legal name | matched GLEIF name="GENMAB A/S" | status=ISSUED | nextRenewal=2026-12-27T14:28:11Z | registeredAs=21023884 | registeredAs filter total=1 LEIs=[529900MTJPDPE4MHJ122] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001434265 | legalName="GENMAB A/S" (total 1) -> ["GENMAB A/S"]
0001002910 | lei=XRZQ5S7HYJFPHJ78L959 | found by=legal name | matched GLEIF name="AMEREN CORPORATION" | status=ISSUED | nextRenewal=2026-12-29T19:36:28Z | registeredAs=00414845 | registeredAs filter total=1 LEIs=[XRZQ5S7HYJFPHJ78L959] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NATURAL_PERSONS
  0001002910 | legalName="AMEREN CORP" (total 0) -> []
  0001002910 | legalName="AMEREN Corporation" (total 2) -> ["AMEREN CORPORATION", "Ameren Corporation Savings Investment Plan - The Ameren Stable Interest Income Fund"]
0001444406 | lei=254900IDGKCJICKBPA66 | found by=legal name | matched GLEIF name="Ecopetrol S.A." | status=ISSUED | nextRenewal=2027-01-10T19:49:23Z | registeredAs=899999068-1 | registeredAs filter total=1 LEIs=[254900IDGKCJICKBPA66] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001444406 | legalName="ECOPETROL S.A." (total 2) -> ["Ecopetrol S.A.", "Pasivos Pensionales Porvenir - Patrimonio Autonomo de Pasivos Pensionales ECOPETROL S.A."]
0001713683 | lei=529900MZ0RTK1BWRNF46 | found by=legal name | matched GLEIF name="ZSCALER, INC." | status=ISSUED | nextRenewal=2027-04-18T17:24:59Z | registeredAs=4431830 | registeredAs filter total=1 LEIs=[529900MZ0RTK1BWRNF46] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001713683 | legalName="Zscaler, Inc." (total 77547) -> ["ZSCALER, INC.", "ZSCALER CANADA, INC.", "Zscaler Switzerland GmbH", "ZSCALER UK LTD.", "ZSCALER AUSTRALIA PTY LTD"]
0000036270 | lei=549300WYXDDBYRASEG81 | found by=legal name | matched GLEIF name="M&T BANK CORPORATION" | status=ISSUED | nextRenewal=2027-02-23T19:39:05Z | registeredAs=284484 | registeredAs filter total=1 LEIs=[549300WYXDDBYRASEG81] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0000036270 | legalName="M&T BANK CORP" (total 0) -> []
  0000036270 | legalName="M T BANK Corporation" (total 1) -> ["M&T BANK CORPORATION"]
0001110803 | lei=SQ95QG8SR5Q56LSNF682 | found by=legal name | matched GLEIF name="ILLUMINA, INC." | status=ISSUED | nextRenewal=2027-04-14T13:53:20Z | registeredAs=3228889 | registeredAs filter total=1 LEIs=[SQ95QG8SR5Q56LSNF682] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0001110803 | legalName="ILLUMINA, INC." (total 77552) -> ["ILLUMINA, INC.", "ILLUMINA HOLDINGS INC.", "Illumina Global Ltd", "Illumina Lighting Limited", "BELLINA ILLUMINA S.R.L."]
0001535759 | lei=5967007LIEEXZXJ9HK73 | found by=legal name | matched GLEIF name="KONGSBERG GRUPPEN ASA" | status=ISSUED | nextRenewal=2027-01-09T12:01:33Z | registeredAs=943753709 | registeredAs filter total=1 LEIs=[5967007LIEEXZXJ9HK73] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001535759 | legalName="Kongsberg Gruppen ASA" (total 1) -> ["KONGSBERG GRUPPEN ASA"]
0001116578 | lei=5493001Z3ZE83NGK8Y12 | found by=legal name | matched GLEIF name="Prudential Public Limited Company" | status=ISSUED | nextRenewal=2027-01-08T00:18:00Z | registeredAs=01397169 | registeredAs filter total=1 LEIs=[5493001Z3ZE83NGK8Y12] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0001116578 | legalName="PRUDENTIAL PLC" (total 3) -> ["AFRICA PRUDENTIAL PLC", "Prudential Funding (Asia) Plc", "THE PRUDENTIAL PLC EMPLOYEE SHARE TRUST"]
  0001116578 | legalName="PRUDENTIAL Public Limited Company" (total 3) -> ["Prudential Public Limited Company", "Prudential Capital Public Limited Company", "Prudential International Assurance Public Limited Company"]
0001406234 | lei=549300WEH5R2OODI7Y90 | found by=legal name | matched GLEIF name="BROOKFIELD INFRASTRUCTURE PARTNERS L.P." | status=LAPSED | nextRenewal=2017-06-13T13:03:00Z | registeredAs=40126 | registeredAs filter total=1 LEIs=[549300WEH5R2OODI7Y90] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0001406234 | legalName="Brookfield Infrastructure Partners L.P." (total 1) -> ["BROOKFIELD INFRASTRUCTURE PARTNERS L.P."]
0001093557 | lei=549300YSK3QDSFR5EU59 | found by=legal name | matched GLEIF name="DEXCOM, INC." | status=ISSUED | nextRenewal=2027-08-06T20:27:51Z | registeredAs=3030192 | registeredAs filter total=1 LEIs=[549300YSK3QDSFR5EU59] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001093557 | legalName="DEXCOM INC" (total 1) -> ["DEXCOM, INC."]
0001009001 | lei=N4BHALMXL3GMZKCUON55 | found by=legal name | matched GLEIF name="CAMECO CORPORATION" | status=ISSUED | nextRenewal=2027-05-08T18:17:56Z | registeredAs=332981-0 | registeredAs filter total=1 LEIs=[N4BHALMXL3GMZKCUON55] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001009001 | legalName="CAMECO CORP" (total 0) -> []
  0001009001 | legalName="CAMECO Corporation" (total 1) -> ["CAMECO CORPORATION"]
0001140536 | lei=549300WHC56FF48KL350 | found by=legal name | matched GLEIF name="WILLIS TOWERS WATSON PUBLIC LIMITED COMPANY" | status=ISSUED | nextRenewal=2027-02-19T14:42:52Z | registeredAs=475616 | registeredAs filter total=1 LEIs=[549300WHC56FF48KL350] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NATURAL_PERSONS
  0001140536 | legalName="WILLIS TOWERS WATSON PLC" (total 0) -> []
  0001140536 | legalName="WILLIS TOWERS WATSON Public Limited Company" (total 1) -> ["WILLIS TOWERS WATSON PUBLIC LIMITED COMPANY"]
0001190723 | lei=549300Y7C05BKC4HZB40 | found by=legal name | matched GLEIF name="TENARIS S.A." | status=ISSUED | nextRenewal=2027-04-21T18:00:00Z | registeredAs=B85203 | registeredAs filter total=1 LEIs=[549300Y7C05BKC4HZB40] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0001190723 | legalName="TENARIS SA" (total 0) -> []
  0001190723 | legalName="TENARIS" (total 6) -> ["TENARIS S.A.", "TENARIS SOLUTIONS URUGUAY S.A.", "TENARIS INVESTMENTS SWITZERLAND AG", "TENARIS GLOBAL SERVICES S.A.", "TENARIS FINANCIAL SERVICES S.A."]
0001324424 | lei=2549009GW3Z3DQCB8H87 | found by=legal name | matched GLEIF name="Expedia Group, Inc." | status=ISSUED | nextRenewal=2027-05-01T17:46:51Z | registeredAs=3956616 | registeredAs filter total=1 LEIs=[2549009GW3Z3DQCB8H87] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NATURAL_PERSONS
  0001324424 | legalName="Expedia Group, Inc." (total 77542) -> ["Expedia Group, Inc.", "INC Group Inc.", "INC", "Gazelle.ia Inc. / Gazelle.ai Inc.", "Pruvations Inc 401K Inc"]
0001666175 | lei=549300MQYQ9Y065XPR71 | found by=legal name | matched GLEIF name="Fortis Inc." | status=ISSUED | nextRenewal=2027-09-25T16:32:28Z | registeredAs=21782 | registeredAs filter total=3 LEIs=[549300MQYQ9Y065XPR71, 969500ZPPO6WBTVPW548, 3912002FCI92HFVQGO30] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001666175 | legalName="Fortis Inc." (total 6) -> ["Fortis Inc.", "FORTIS 333, INC.", "Fortis Investments Inc.", "FORTIS VL INC.", "FORTIS CAPITAL STRATEGIES INC."]
0001140022 | lei=YF0Y5B0IB8SM0ZFG9G81 | found by=legal name | matched GLEIF name="AVIVA PLC" | status=ISSUED | nextRenewal=2026-12-31T00:00:00Z | registeredAs=02468686 | registeredAs filter total=1 LEIs=[YF0Y5B0IB8SM0ZFG9G81] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0001140022 | legalName="AVIVA PLC" (total 2) -> ["AVIVA PLC", "Aviva Investors Liquidity Funds plc - Aviva Investors Sterling Core Liquidity Fund"]
0001030894 | lei=549300J3CG5T6RZWLN53 | found by=legal name | matched GLEIF name="CELESTICA INC." | status=ISSUED | nextRenewal=2027-10-06T19:00:30Z | registeredAs=1201522 | registeredAs filter total=1 LEIs=[549300J3CG5T6RZWLN53] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0001030894 | legalName="CELESTICA INC" (total 1) -> ["CELESTICA INC."]
0001038683 | lei=635400BR2ROC1FVEBQ56 | found by=legal name | matched GLEIF name="Ryanair Holdings Public Limited Company" | status=ISSUED | nextRenewal=2027-12-21T00:00:00Z | registeredAs=249885 | registeredAs filter total=1 LEIs=[635400BR2ROC1FVEBQ56] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001038683 | legalName="RYANAIR HOLDINGS PLC" (total 0) -> []
  0001038683 | legalName="RYANAIR HOLDINGS Public Limited Company" (total 1) -> ["Ryanair Holdings Public Limited Company"]
0000920148 | lei=549300CDU4WF6Q2YMS76 | found by=former name | matched GLEIF name="Laboratory Corporation of America Holdings" | status=DUPLICATE | nextRenewal=2014-06-05T17:16:00Z | registeredAs= | registeredAs filter total=null LEIs=[] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=none
  0000920148 | legalName="LABCORP HOLDINGS INC." (total 0) -> []
  0000920148 | legalName="LABCORP HOLDINGS Incorporated" (total 0) -> []
  0000920148 | legalName="LABCORP HOLDINGS" (total 2) -> ["LABCORP INTERNATIONAL HOLDINGS LIMITED", "Labcorp International Holdings B.V."]
  0000920148 | legalName="LABORATORY CORP OF AMERICA HOLDINGS" (former name "LABORATORY CORP OF AMERICA HOLDINGS") (total 0) -> []
  0000920148 | legalName="LABORATORY Corporation OF AMERICA HOLDINGS" (former name "LABORATORY CORP OF AMERICA HOLDINGS") (total 2) -> ["Laboratory Corporation of America Holdings", "LABORATORY CORPORATION OF AMERICA HOLDINGS"]
0000731802 | lei=QVLWEGTD2S8GJMO8D383 | found by=legal name | matched GLEIF name="ATMOS ENERGY CORPORATION" | status=ISSUED | nextRenewal=2027-08-07T17:37:42Z | registeredAs=0054895300 | registeredAs filter total=1 LEIs=[QVLWEGTD2S8GJMO8D383] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0000731802 | legalName="ATMOS ENERGY CORP" (total 0) -> []
  0000731802 | legalName="ATMOS ENERGY Corporation" (total 1) -> ["ATMOS ENERGY CORPORATION"]
0001383650 | lei=5493005UEC8AZ34LDV29 | found by=legal name | matched GLEIF name="CHENIERE ENERGY PARTNERS, L.P." | status=ISSUED | nextRenewal=2027-10-25T00:00:00Z | registeredAs=4208394 | registeredAs filter total=1 LEIs=[5493005UEC8AZ34LDV29] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_LEI
  0001383650 | legalName="Cheniere Energy Partners, L.P." (total 25265) -> ["CHENIERE ENERGY PARTNERS, L.P.", "Cheniere Energy Partners LP Holdings, LLC", "L.P", "Nuverna, L.P.", "Ascona L.P."]
0000719955 | lei=549300IARG6YWVTZ1I92 | found by=legal name | matched GLEIF name="Williams-Sonoma, Inc." | status=LAPSED | nextRenewal=2014-03-27T17:59:00Z | registeredAs=4903496 | registeredAs filter total=1 LEIs=[549300IARG6YWVTZ1I92] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_LEI
  0000719955 | legalName="WILLIAMS SONOMA INC" (total 2) -> ["Williams-Sonoma, Inc.", "Williams-Sonoma Canada, Inc."]
0001637459 | lei=9845007488EC87F5AF14 | found by=legal name | matched GLEIF name="THE KRAFT HEINZ COMPANY" | status=ISSUED | nextRenewal=2027-06-28T16:54:47Z | registeredAs=5286651 | registeredAs filter total=1 LEIs=[9845007488EC87F5AF14] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001637459 | legalName="Kraft Heinz Co" (total 0) -> []
  0001637459 | legalName="Kraft Heinz Company" (total 5) -> ["THE KRAFT HEINZ COMPANY", "Kraft Heinz Foods Company", "Kraft Heinz Foods Company L.P.", "Kraft Heinz Company Master Retirement Trust", "Kraft Heinz Company Retiree Health & Welfare Benefits Trust III"]
0001410636 | lei=549300DXHIJQMD5WFW18 | found by=legal name | matched GLEIF name="AMERICAN WATER WORKS COMPANY, INC." | status=ISSUED | nextRenewal=2027-08-29T21:01:34Z | registeredAs=352210 | registeredAs filter total=1 LEIs=[549300DXHIJQMD5WFW18] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001410636 | legalName="American Water Works Company, Inc." (total 77542) -> ["AMERICAN WATER WORKS COMPANY, INC.", "American Water Works Company Inc. - Post Retirement Medical Trust / Bargaining", "INC Group Inc.", "INC", "Gazelle.ia Inc. / Gazelle.ai Inc."]
0000886986 | lei=T8KI5SQ2JRWHL7XY0E11 | found by=legal name | matched GLEIF name="Teck Resources Limited" | status=ISSUED | nextRenewal=2027-10-17T18:56:38Z | registeredAs=446056-1 | registeredAs filter total=1 LEIs=[T8KI5SQ2JRWHL7XY0E11] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0000886986 | legalName="TECK RESOURCES LTD" (total 0) -> []
  0000886986 | legalName="TECK RESOURCES Limited" (total 2) -> ["Teck Resources Limited", "Pension Plan for Executive and Qualified Senior Employees of Teck Resources Limited and Associated Companies"]
0001175454 | lei=549300DG6RR0NQSFLN74 | found by=legal name | matched GLEIF name="CORPAY, INC." | status=ISSUED | nextRenewal=2027-11-06T10:12:25Z | registeredAs=2854298 | registeredAs filter total=1 LEIs=[549300DG6RR0NQSFLN74] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001175454 | legalName="CORPAY, INC." (total 77544) -> ["CORPAY, INC.", "CORPAY ONE, INC.", "Corpay Trading Canada Inc.", "CORPAY (NZ) LIMITED", "CORPAY TECHNOLOGIES OPERATING COMPANY, LLC"]
0000029534 | lei=OPX52SQVOZI8IVSWYU66 | found by=legal name | matched GLEIF name="DOLLAR GENERAL CORPORATION" | status=ISSUED | nextRenewal=2027-04-22T21:04:21Z | registeredAs=000351611 | registeredAs filter total=1 LEIs=[OPX52SQVOZI8IVSWYU66] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0000029534 | legalName="DOLLAR GENERAL CORP" (total 0) -> []
  0000029534 | legalName="DOLLAR GENERAL Corporation" (total 1) -> ["DOLLAR GENERAL CORPORATION"]
0000313216 | lei=H1FJE8H61JGM1JSGM897 | found by=legal name | matched GLEIF name="Koninklijke Philips N.V." | status=ISSUED | nextRenewal=2027-06-26T09:11:11Z | registeredAs=17001910 | registeredAs filter total=1 LEIs=[H1FJE8H61JGM1JSGM897] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0000313216 | legalName="KONINKLIJKE PHILIPS NV" (total 0) -> []
  0000313216 | legalName="KONINKLIJKE PHILIPS" (total 1) -> ["Koninklijke Philips N.V."]
0000900075 | lei=549300KVYX3JWMYEHU61 | found by=legal name | matched GLEIF name="COPART, INC." | status=ISSUED | nextRenewal=2027-02-07T20:43:14Z | registeredAs=5030359 | registeredAs filter total=1 LEIs=[549300KVYX3JWMYEHU61] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0000900075 | legalName="COPART INC" (total 1) -> ["COPART, INC."]
0001094285 | lei=549300VSMO9KYQWDND94 | found by=legal name | matched GLEIF name="TELEDYNE TECHNOLOGIES INCORPORATED" | status=ISSUED | nextRenewal=2027-06-10T15:05:21Z | registeredAs=3083054 | registeredAs filter total=1 LEIs=[549300VSMO9KYQWDND94] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0001094285 | legalName="TELEDYNE TECHNOLOGIES INC" (total 0) -> []
  0001094285 | legalName="TELEDYNE TECHNOLOGIES Incorporated" (total 2) -> ["TELEDYNE TECHNOLOGIES INCORPORATED", "Teledyne Technologies Incorporated Defined Benefit Master Trust"]
0001781335 | lei=549300ZLBKR8VSU25153 | found by=legal name | matched GLEIF name="OTIS WORLDWIDE CORPORATION" | status=ISSUED | nextRenewal=2027-07-14T20:11:00Z | registeredAs=7283745 | registeredAs filter total=1 LEIs=[549300ZLBKR8VSU25153] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NON_CONSOLIDATING
  0001781335 | legalName="Otis Worldwide Corp" (total 0) -> []
  0001781335 | legalName="Otis Worldwide Corporation" (total 1) -> ["OTIS WORLDWIDE CORPORATION"]
0001769628 | lei=984500511DP2B6186053 | found by=legal name | matched GLEIF name="COREWEAVE, INC." | status=ISSUED | nextRenewal=2027-05-13T17:02:29Z | registeredAs=6551467 | registeredAs filter total=1 LEIs=[984500511DP2B6186053] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001769628 | legalName="CoreWeave, Inc." (total 77546) -> ["COREWEAVE, INC.", "COREWEAVE FINANCING DDTL V, LLC", "COREWEAVE FINANCING DDTL V-V, LLC", "CoreWeave Compute Acquisition Co. VIII, LLC", "CoreWeave Compute Acquisition Co. VII, LLC"]
0001001290 | lei=529900UYAEYQCQ2BKB17 | found by=legal name | matched GLEIF name="CREDICORP LTD." | status=ISSUED | nextRenewal=2027-09-09T12:54:46Z | registeredAs=21045 | registeredAs filter total=2 LEIs=[529900UYAEYQCQ2BKB17, 213800RULAHC9K2OI278] | fields used: entity.legalName, entity.registeredAs, registration.status, registration.nextRenewalDate | parent lei=(none) parent name=(none) | exception=DIRECT_ACCOUNTING_CONSOLIDATION_PARENT: NO_KNOWN_PERSON
  0001001290 | legalName="CREDICORP LTD" (total 2) -> ["CREDICORP LTD.", "Credicorp Capital Ltd."]

FAILED SOURCES (after one retry, with what was tried):
(none)
```

## DATA FILES

```synmerco-data
1348a9d89bc3a23f6994b7d43ce917aaba58ea963a6e5b9a6598b934121fc5fa gleif-400-pull1.csv
67cf76ab946c836f537f5cb6271cf77082c67d80580db566e87d4f642ab04a3d gleif-400-pull2.csv
67cf76ab946c836f537f5cb6271cf77082c67d80580db566e87d4f642ab04a3d gleif-400-pull3.csv
```
