# WISER-Training-Modules-
WISER Synthetic Dataset Package for Modules 4-8

This package contains five fully synthetic CSV datasets for WISER Modules 4-8:

Dataset	Intended use
data/post_overdose_data.csv	Module 5 visualization, overdose surveillance, provisional-data caveats, and equity overlays
data/encounters.csv	Cross-module encounter-level substrate for clinical, SDOH, referral, and follow-up activities
data/notes.csv	Module 4 NLP semantics, terminology crosswalks, stigma-free language review, and text extraction
data/insurance.csv	Insurance access, prior authorization, MOUD coverage, and access-barrier activities
data/hopebridge_ml.csv	Module 6 HopeBridge ML workflow for prediction, subgroup performance, and fairness auditing

Important use notes
-	These records are synthetic and are not derived from any real patient, clinician, institution, or health system.
-	Do not use these data for clinical decision-making, population estimation, publication as real-world evidence, or operational planning.
-	Variables use person-first and stigma-free terminology where possible. A small number of legacy terms appear only in notes.csv for NLP crosswalk and language-audit teaching activities.
-	The package avoids direct identifiers and does not contain PHI.
-	Synthetic IDs are internally linkable across files via patient_id, and notes can link to encounters via encounter_id.
Hosting for Google Colab

Option A: GitHub raw URLs
1.	Create a GitHub repository, for example wiser-course-data.
2.	Upload the contents of this package.
3.	For each CSV, click Raw on GitHub and copy the raw URL.
4.	In each notebook, set DATA_URL to the raw URL.

Example:

DATA_URL = https://github.com/caracarlin/WISER-Training-Modules-

notes = pd.read_csv(DATA_URL)
Option B: Google Drive
1.	Upload the CSV files to a shared Google Drive folder.
2.	Set sharing to "Anyone with the link can view" if institutional policy allows.
3.	Use gdown or the Google Drive file ID in Colab.

Example:

!pip -q install gdown

!gdown --id FILE_ID -O notes.csv

notes = pd.read_csv("notes.csv")

Option C: LMS or institutional file hosting
Upload the CSV files to your LMS/course file area or institutional web storage. Use HTTPS links that are accessible from Colab without login, or instruct learners to upload the files manually.

Suggested notebook URL mapping
Notebook	Dataset URL to use

Module 4 NLP	data/notes.csv
Module 5 Visualization	data/post_overdose_data.csv
Module 6 Machine Learning	data/hopebridge_ml.csv
Module 7 Deep Learning & Images	no CSV required for template; optional use of data/encounters.csv for reflection metadata
Module 8 Capstone	all CSVs as optional integrated evidence sources

Stigma-free language reference
Use person-first language such as "person with opioid use disorder," "person with a substance 
use disorder," "substance use," "positive toxicology result," and "negative toxicology result." 
Avoid terms such as "addict," "drug abuser," and "clean/dirty" for toxicology results. 
See NIDA's Words Matter guidance: https://nida.nih.gov/nidamed-medical-health-professionals/health-professions-education/words-matter-terms-to-use-avoid-when-talking-about-addiction

Files
-	dataset_manifest.csv: row and column counts for each dataset
-	data/: five synthetic CSV datasets
-	data_dictionaries/: one data dictionary CSV per dataset
-	docs/schema_overview.md: compact schema overview
-	docs/colab_data_urls_template.md: copy/paste placeholders for notebook DATA_URL values

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
(https://colab.research.google.com/drive/1ST-e-TrCMB1hyw_4-wHFbdZlCcwwrymj?usp=sharing))
