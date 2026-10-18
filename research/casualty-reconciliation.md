# Civilian and military casualties: preliminary reconciliation

**Checkpoint:** 02 · **Evidence cutoff:** 19 October 2026  
**Status:** Dated public claims register only. NOT a verified census of the dead and injured.

## Reconciliation rule

Each published figure needs reporting date, incident period, side, civilian/military distinction, killed/injured distinction, source, causal allegation, and whether it supersedes earlier cumulative data. A number reported twice through the same military release is **one source**, not two independent confirmations. We do not add earlier daily claims into later cumulative claims.

## Comparable public statements, 11–13 May 2025

| Side | Population | Killed as officially reported | Injured as officially reported | Report as of | Provenance |
|---|---|---:|---:|---|---|
| Pakistan | Civilian | 40 | 121 | 13 May | ISPR via [APP](https://www.app.com.pk/national/40-civilians-11-troops-martyred-in-indian-aggression-ispr/), S44 |
| Pakistan | Military | 11 | 78 | 13 May | Same release, S44 |
| India | Civilian | At least 16 | Not established as a matching 13 May cumulative figure | Reuters 13 May | [Reuters](https://www.reuters.com/world/asia-pacific/pakistan-says-clashes-with-neighbour-india-killed-more-than-50-2025-05-13/), S43 |
| India | Military | 5 | Not established in current evidence pass | Indian briefing 11 May, Reuters 13 May | [AP](https://apnews.com/article/6fa80010fa8ffee1da1f28e7b593aa2d), [Reuters](https://www.reuters.com/world/asia-pacific/pakistan-says-clashes-with-neighbour-india-killed-more-than-50-2025-05-13/), S52/S43 |

These totals, as reported by the governments, give a **minimum provisional aggregate of 72 deaths** (51 reported by Pakistan, at least 21 by India) if the cited categories are non-overlapping and share the same conflict scope. This is **not** a rigorously verified combined death toll and **must not** be published as an independently established result.

### Important date and scope caveats

- India's 8 May [MEA/PIB reporting](https://www.mea.gov.in/Speeches-Statements.htm?dtl%2F39478=) stated 16 Indian civilian deaths and 59 injuries at that time. It cannot automatically be assigned to the end of the conflict or added to another cumulative number.
- Pakistan's 13 May statement reported 40 civilian deaths **and** 11 military deaths. Reporting "40 killed in Pakistan" without specifying civilians undercounts the official announcement.
- Five PAF personnel were listed among Pakistan's 11 military fatalities in the ISPR May 13 account. A 14 May [Washington Post](https://www.washingtonpost.com/world/2025/05/14/india-pakistan-strikes-conflict-damage/) account attributed six PAF deaths to the military and site locations. The discrepancy remains unresolved pending original release revision and name reconciliation.
- A Pakistani military death at a damaged airfield is not proof that an aircraft was inside a destroyed hangar. Do not infer equipment loss from fatalities.
- Incident-specific reports of deaths near a crash site may involve post-crash hazards, rather than intentional strikes, and require a distinct causal category.
- Fatalities in the 22 April Pahalgam attack are **separate** from May 7–10 conflict casualties and must not be appended to war-fighting casualties without an explicitly defined broader time scope.

## Wording and scope contradiction in India's own official record

India's [Defence Minister's 28 July parliamentary statement](https://www.pib.gov.in/PressReleasePage.aspx?PRID=2149356&lang=2&reg=48) described no Indian military casualties **during Operation Sindoor**. However, India’s [11 May joint military briefing as reported by AP](https://apnews.com/article/6fa80010fa8ffee1da1f28e7b593aa2d) publicly reported **five Indian soldiers killed** in the broader hostilities. Without the original unedited wording and date/incident details, the statements may reflect different definitions of the operation and wider fighting. They should not be reconciled by silently changing five to zero or assumed to prove deliberate misinformation.

The project's cumulative casualty table therefore retains the five **reported** Indian military deaths and separately records the minister's limited phrase as a contradiction requiring scope clarification.

## Demonstrable physical impact versus reported death

Evidence of damage to school structures, religious buildings, civilian dwellings and infrastructure exists in independent and local reportage. Each damage event must be linked to date, safe-location granularity and public photos. None should be used to infer an uncounted death without a reliable person- or hospital-level record.

## Source lineage and overlap

- APP and Radio Pakistan reports repeating ISPR numbers are the same underlying announcement.
- Reuters' report of ISPR totals is an independent account of a *government statement*, not an independent body count.
- The Washington Post's airfield damage review used satellite data independent of ISPR, but its description of personnel fatalities still relies on ISPR.
- May 8 Indian and May 13 Indian numbers are non-independent chronology points with potential overlap.

## Future casualty dataset schema

`event_id`, `date_range`, `side`, `district`, `incident_type`, `status`, `killed`, `injured`, `population`, `source_id`, `report_date`, `underlying_authority`, `duplicate_group`, `clinical_confirmation`, `causal_uncertainty`, `notes`, `last_reviewed`.

Do not publish protected witnesses, unnecessary home addresses or private medical details.

## Open questions

1. What names, administrative records and medical evidence support the civilian numbers on both sides?
2. Were later corrections made after May 13?
3. Were deaths from the initial 7 May strikes separated from later cross-border fire and airfield attacks?
4. How many military and civilian injuries were sustained, and how many subsequently resulted in deaths?
5. Why do five and six PAF death counts appear in two different dated sources?
6. Did the declared ceasefire's reported violation incidents cause further casualties after 17:00 IST?

## Related dataset

Machine-readable four aggregate statements: [data/research.json](../data/research.json), `casualties` collection. No deduplicated person-level ledger exists yet.
