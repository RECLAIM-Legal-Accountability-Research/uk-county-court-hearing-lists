Longitudinal Collection of UK County Court Daily Hearing Lists  
<https://doi.org/10.5281/zenodo.19828688>  
Published April 28, 2026 | Version v1 | Dataset  Open  
Authors/Creators: Bohlinger, Britta (Researcher)  
# APA citation:
Bohlinger, B. (2026). Longitudinal Collection of UK County Court Daily Hearing Lists [Data set]. Zenodo. <https://doi.org/10.5281/zenodo.19828688>  

GitHub <https://github.com/BebeHub/UK-County-Court-Daily-Hearing-Lists/>

# Description
Purpose and Global Accessibility
This project provides an independent archive to support Access to Justice for the public, including researchers, NGOs, and the growing number of self-represented parties, i.e. Litigants in Person (LIPs) also known as pro-se litigants, globally.
 
By offering this data in a machine-readable format (pipe-separated, fixed width) with comparative terminology, the project ensures that practices, patterns and allocation of time in County Courts remain in the public domain and inform applications, decision-making processes and related complaints processes, as well as appeals or actions required to address irregularities.
 
Governance and Funding
The research project has been independently conceived, designed, and executed, including all necessary personal funding for data acquisition and processing. The project maintains full autonomy over the research agenda, data interpretation, and final outputs.
 
Human-AI Collaborative Framework
To ensure methodological rigour and reduce potential cognitive bias, a hybrid workflow integrating Large Language Models (LLMs) alongside traditional data analysis tools was employed. This collaboration was structured as an iterative, Agile-based review cycle, where AI assisted in:  

Data Aggregation: Consolidating raw listings from multiple County Courts, including Central London, Wandsworth, and Clerkenwell & Shoreditch into standardised, fixed-width plain text tables.  

Trend Identification: Recognising longitudinal patterns, such as the regular bi-monthly processing of "Restored Name" applications and the consistency of "HMRC Petitions" peaks.  

Verification: Cross-referencing AI-generated subtotals against source records to ensure accuracy in unique case reference counts and hearing channel classifications (e.g., In Person, CVP / MS Teams, Telephone, and On the Papers).  

By consolidating data from July 2025 through April 2026, this archive serves as a public resource for researchers, litigants, NGOs and other parties globally. 
 
Case management patterns vary, depending on the allocated track (based on case value in £/GBP) and judicial allocation of time. Judicial determinations "On the Papers" permit maximum flexibility as they do not require parties in attendance. The dataset makes this granular, anonymised data transparent and searchable beyond the fragmented official portals which override daily listings.
 
Disclaimer: The comparative legal terminology provided here, and all other information within this dataset and research project, is for archival and informational purposes only. It does not constitute legal advice, legal strategy, or financial advice.

Methodology:
This dataset consists of data extracted and synthesised from official UK County Court Daily Hearing / Cause Lists (July 2025 – April 2026).  The primary source data are not included in this repository to respect the terms of the original listing services.
 
The data has been transformed into a structured format to facilitate longitudinal analysis of hearing types, and the use of remote hearing channels including video, telephone and on the papers.  

Distinct Entities: It distinguishes between the total number of entries and the number of specific, separate categories. For instance, while there are hundreds of individual hearings, they only occupy five unique channels, i.e. In person, MS Teams / CVP, On the Papers, and Telephone.

Methodological Rigour: Using "unique" ensures counting of discrete variables rather than raw instances. The sources themselves adopt this terminology, specifically defining "Count" as the total number of "unique case reference numbers" to avoid double-counting the same legal matter in aggregated summaries.

Longitudinal Accuracy: Across the various date ranges - from July 2025 through April 2026 - certain courts or types appear repeatedly. Identifying the unique count (e.g., six courts) provides exactly how many distinct venues are being monitored regardless of how many times they appear in the data.  

Technical specification  
Standardised `.txt` File Format Specification to ensure the dataset is machine-readable and archival-grade. Structural rules applied:

1. Fixed-Width Layout
- Structure: Uses a fixed-width plain text table where each column has a consistent character count.
- Separator: Uses the pipe symbol (`|`) between headers and data columns to facilitate future conversion to CSV or database formats.
- Headers: Uses exactly these six column headers:
    `DATE       | COURT NAME               | HEARING TYPE             | CATEGORY         | CHANNEL       | COUNT`
 
2. Column Definitions
- DATE: DD/MM/YYYY.
- COURT NAME: The full name of the court (e.g., Central London, Wandsworth).
- HEARING TYPE: The primary description of the hearing (e.g., Application, Trial).
- CATEGORY: The bracketed legal classification found in the source (e.g., [PCOL], [Small Claim]). Uses `[N/A]` if not present.
- CHANNEL: The mode of appearance (e.g., In person, MS Teams / CVP [Cloud Video Platform], On the Papers).
- COUNT: The total number of unique case reference numbers listed for that specific row profile.
 
3. Privacy and Anonymisation
- No Personal Data: Removed were all names of Judges, District Judges, Clerks, Ushers, and Parties. 
- Data Aggregation: Only includes counts of cases per hearing profile; does not list individual case names or numbers.
 
4. Asterisked Comments (Footer)
Qualitative administrative metadata that does not fit into the table has been placed at the bottom of the file using a single or double asterisk system (*Comment regarding specific administrative list or venue; ** Comment regarding specific officer or listing anomaly].

# Standardized Template  
```text
DATE       | COURT NAME               | HEARING TYPE             | CATEGORY         | CHANNEL       | COUNT
-------------------------------------------------------------------------------------------------------------
DD/MM/YYYY | [Full Court Name]        | [Type of Hearing]        | [Tag]            | [In person/Remote]| 0
-------------------------------------------------------------------------------------------------------------
TOTAL FOR DATE                                                                                        0
```
Technical info (English)
This analysis, supported by Notebook LM (AI Assistant), demonstrates how the raw text of the daily hearing [cause] lists can be transformed into a machine-readable format for statistical research on court operations, administrative backlog, and the use of remote hearing technologies [channels].

Notebook LM (Language Model) relies on source-grounded AI and uses only the documents uploaded by the user.  In this case only PDF documents were in scope. This significantly reduced AI "hallucinations", ensuring a higher degree of accuracy, and minimising the subsequent manual quality checks and corrections.

# Table of contents (English)  
DT_ST	DT_EN	FILE_NAME  
28/04/26	28/04/2026	20260428_CC HearingListing_AggregatedData.txt  
17/04/26	21/04/2026	20260417-21_CCHearingListing_Aggregated Data.txt  
17/11/25	25/03/2026	20260325_20251117_CCHearingList_AggregatedData.txt  
22/09/25	14/11/2025	20250922-14112025_CCHearingList_AggregatedData.txt  
10/07/25	18/09/2025	20250710-18092025_CCHearingListing_AggreatedData.txt  

# Methods (English)
Dictionary - Comparative Legal and Institutional Terminology  
The comparative legal terminology provided here, and all other information within this data set and research project, is for archival and informational purposes only. It does not constitute legal advice, legal strategy, or financial advice.  
  
Note: German terms use the grammatical masculine form (m) for brevity and indexing consistency; these terms are intended to be gender-neutral and apply to all parties regardless of gender.
 
| Key Term (UK) | Equivalent (USA) | Equivalent (Germany) |
| :--- | :--- | :--- |
| Application | Motion | Antrag |
| Claim | Lawsuit / Action | Gerichtsfall / Klage |
| Claimant | Plaintiff | Kläger (m) |
| County Court | District/County Court | Amtsgericht |
| Defendant | Defendant | Beklagter (m) |
| DWP (Welfare/Pensions) | Social Security Admin. | Deutsche Rentenversicherung |
| Hearing Channel | Hearing Mode | Verhandlungsform |
| HMCTS Staff / Civil Servant | Court Clerk / Public Servant | Justizverwaltungsangestellter (m) / Beamter (m) |
| HMCTS | Court Administration | Justizverwaltung |
| HMRC (Tax/Revenue) | IRS | Finanzamt |
| Judgement | Judgment | Gerichtsurteil |
| Legal Aid | Legal Services / Pro Bono | Prozesskostenbeihilfe |
| Litigant in Person | Pro se Litigant | Selbstvertreter (m) |
| Local Authority | Municipal Government | Kommunalbehörde |
| Official Receiver | Bankruptcy Trustee | Insolvenzverwalter (m) |
| On the Papers | Submission on Briefs | Entscheidung nach Aktenlage |
| Parties | Parties | Klageparteien |
| Possession | Eviction / Foreclosure | Räumung / Besitzentziehung |
| Public Examination | Creditors' Meeting | Öffentliche Befragung |
| Self-represented | Pro se | Selbstvertretend |
| Solicitor / Barrister | Attorney / Lawyer | Rechtsanwalt (m) |
| Statement of Claim | Complaint | Klageschrift |
| University Hospital | Public Hospital | Universitätsklinikum |
 
# Note on the Administration of Justice and the Judiciary:
HMCTS (Her Majesty’s Courts and Tribunals Service) is an executive agency of the Ministry of Justice (MoJ). Its staff handle administrative listings, have limited powers, are civil servants, and distinct, from the independent judiciary. HMCTS, i.e. the Administration of Justice, are not legally trained and do not have powers to substitute judicial decision-making.  HMCTS are not authorised to issue legally binding rulings such as judicial orders and judgments.
 
HMCTS are required to comply with statutory requirements and the legal framework, including the Civil Procedure Rules (CPR), Equality Act 2010, Care Act 2014, Public Records Act 1958, Data Protection Act 2018 and GDPR, Freedom of Information Act 2000 (FoIA), Courts Act 2003, Data Protection rules and further frameworks, regulations and rules. HMCTS are restricted to administrative tasks and specified, authorised functions; HMCTS are not authorised to provide legal advice or act as legal representatives. 
 
HMCTS is accountable to the UK Parliament.  Its Justice Committee "examines the policies and spending of the Ministry of Justice (and associated public bodies). This includes courts, legal aid, prisons, probation and the rule of law. It also advises on sentencing guidelines." (see "dysfunctional county court system" press release and related letters, reports etc below).

Relevant specific References:
The Bar Council Warning (The BC represents the profession, i.e. barristers)
Bar Council. (2025, July 23). Chronically under-resourced county court system is eroding justice, Bar Council warns. <https://www.barcouncil.org.uk/resource/chronically-under-resourced-county-court-system-is-eroding-justice-bar-council-warns.html>

HMCTS Framework Document
Ministry of Justice & HM Courts & Tribunals Service. (2014). HMCTS framework document. <https://assets.publishing.service.gov.uk/media/5a7efae440f0b6230268cbeb/hmcts-framework-document-2014.pdf>

HMCTS Equality and Diversity Policy
HM Courts & Tribunals Service. (n.d.). Equality and diversity. GOV.UK. <https://www.gov.uk/government/organisations/hm-courts-and-tribunals-service/about/equality-and-diversity>

Justice Committee Press Release
Justice Committee. (2025, July 23). Justice denied: dysfunctional county court system failing to deliver justice and requires urgent review, Committee warns. UK Parliament. <https://committees.parliament.uk/committee/102/justice-committee/news/208478/justice-denied-dysfunctional-county-court-system-failing-to-deliver-justice-and-requires-urgent-review-committee-warns/>
 
Law Society of Ireland Gazette Article
Law Society Gazette. (2025, July 23). England and Wales: civil justice dysfunctional. <https://www.lawsociety.ie/gazette/top-stories/2025/july/england-and-wales-civil-justice-dysfunctional/>
 
Supreme Court Scam Alert
Supreme Court of the United Kingdom. (n.d.). Scam alert. <https://supremecourt.uk/scam>

# Notes (English)
Common Latin Terms across Jurisdictions: UK, USA, and Germany

| Latin Term | All 3? | Core Meaning | Jurisdictional Nuance |
| :--- | :--- | :--- | :--- |
| **Ad litem** | Yes | For the suit | Often refers to a guardian appointed for the case's duration. |
| **Bona fide** | Yes | In good faith | German law relates this to *Treu und Glauben* (§ 242 BGB). |
| **De minimis** | Yes | Trifling matters | Used in **Small Claims** where damages are negligible. |
| **Ex parte** | Yes | Without notice | In the UK, modern CPR uses "Without Notice," but the Latin persists. |
| **In camera** | Yes | In private | UK courts increasingly use "In Private" for these hearings. |
| **Inter alia** | Yes | Among other things | Frequently used when listing multiple claims or parties. |
| **Ipso facto** | Yes | By the fact itself | Often used in **Insolvency** regarding automatic contract termination. |
| **Prima facie** | Yes | At first sight | Refers to sufficient evidence to establish a case (e.g., in **Petitions**). |
| **Pro bono** | Yes | For the public good | Legal work done without charge for those without **Legal Aid**. |
| **Pro rata** | Yes | Proportionately | Critical in **HMRC and Creditor Petitions** for asset distribution. |
| **Pro se** | Yes* | For oneself | Standard in USA; known as **Litigant in Person** in the UK. |
| **Quantum** | Yes | Amount | Specifically the financial value of a **Claim** or damages. |
| **Res judicata** | Yes | Already judged | In Germany, referred to as *Rechtskraft* (legal force). |
| **Ultra vires** | Yes | Beyond powers | Used to challenge **Local Authority** actions beyond their scope. |
| **Versus (v)** | Yes | Against | The universal shorthand for designating opposing **Parties**. |

*   **Ex parte:** While still used, it is formally known as a **"Without Notice"** application. These are frequent in emergency **Gas/Electrical Injunctions** within the dataset where the defendant is not present.
*   **In camera:** This has been largely replaced by the term **"In Private."** Many **Family and Public Law** matters use this status to protect parties, particularly in remote **CVP/MS Teams** hearings.
*   **Quantum:** This remains the standard term for the financial assessment of a claim. It is the primary focus of **Fast-track** and **Small Claims** trials, where the court must determine the specific damages to be paid.

Files
20260325_20251117_CCHearingList_AggregatedData.txt  
20250710-18092025_CCHearingListing_AggreatedData.txt  
20250922-14112025_CCHearingList_AggregatedData.txt  
20260325_20251117_CCHearingList_AggregatedData.txt  
20260417-21_CCHearingListing_Aggregated Data.txt  
20260428_CC HearingListing_AggregatedData.txt  

# Related works
Is supplemented by Dataset: 10.5281/zenodo.19697776 (DOI)
Dates Created: 2026-04-28  
APA citation: Bohlinger, B. (2026). Digital Archive of UK Judicial Directories: Point-in-Time Capture (2020, 2025, 2026) [Data set]. Zenodo. <https://doi.org/10.5281/zenodo.19697776>

# References
Courts and Tribunals Judiciary. (n.d.). County court. <https://www.judiciary.uk/courts-and-tribunals/county-court/>. Retrieved April 28, 2026.  
HM Courts & Tribunals Service. (n.d.). Find a court or tribunal. GOV.UK. Retrieved April 28, 2026, from <https://www.gov.uk/find-court-tribunal>  
HM Courts & Tribunals Service (HMCTS). (2025, April 4). List of civil court forms arranged by subject matter [Guidance]. GOV.UK. <https://www.gov.uk/government/publications/civil-procedure-rules-court-forms/list-of-civil-court-forms-arranged-by-subject-matter>  
HM Courts & Tribunals Service (HMCTS). (n.d.). HMCTS hearing lists [Collection]. GOV.UK. Retrieved April 28, 2026, from <https://www.gov.uk/government/collections/hmcts-hearing-lists>  
House of Commons Justice Committee. (2025, July 21). Work of the County Court (HC 677, Fourth Report of Session 2024–25). UK Parliament. <https://publications.parliament.uk/pa/cm5901/cmselect/cmjust/677/report.html>  
House of Lords Constitution Committee. (2025, November 20). The rule of law: holding the line against tyranny and anarchy (HL Paper 211, 13th Report of Session 2024–26). UK Parliament. <https://publications.parliament.uk/pa/ld5901/ldselect/ldconst/211/21102.htm>  
House of Lords Constitution Committee. (2025, November 20). Rule of law: holding the line between anarchy and tyranny [Press release]. UK Parliament. <https://committees.parliament.uk/committee/172/constitution-committee/news/210496/rule-of-law-holding-the-line-between-anarchy-and-tyranny/>  
Magrath, P. (2022, May 5). Court hearing lists and open justice. The Transparency Project. <https://transparencyproject.org.uk/court-hearing-lists-and-open-justice/>  
Ministry of Justice. (2021, November 1). Written submission from the Ministry of Justice [Written evidence submitted to the House of Commons Justice Committee inquiry into supporting open justice and court reporting]. UK Parliament. <https://committees.parliament.uk/writtenevidence/40597/html/>  
Ministry of Justice. (2023). Open justice: The way forward – Call for evidence. UK Government. https://assets.publishing.service.gov.uk/media/645ba3532226ee00130ae5fb/open-justice-cfe.pdf>  
Zenodo. (2025, January 7). Guidelines for describing research data. Zenodo. <https://doi.org/10.5281/zenodo.14609589>
