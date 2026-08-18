WISER-Training-Modules-

WISER Synthetic Dataset Package for Modules 4-8

This package contains five fully synthetic CSV datasets for WISER Modules 4-8:

Dataset Intended use data/post_overdose_data.csv Module 5 visualization, overdose surveillance, provisional-data caveats, and equity overlays data/encounters.csv Cross-module encounter-level substrate for clinical, SDOH, referral, and follow-up activities data/notes.csv Module 4 NLP semantics, terminology crosswalks, stigma-free language review, and text extraction data/insurance.csv Insurance access, prior authorization, MOUD coverage, and access-barrier activities data/hopebridge_ml.csv Module 6 HopeBridge ML workflow for prediction, subgroup performance, and fairness auditing

Important use notes

These records are synthetic and are not derived from any real patient, clinician, institution, or health system.
Do not use these data for clinical decision-making, population estimation, publication as real-world evidence, or operational planning.
Variables use person-first and stigma-free terminology where possible. A small number of legacy terms appear only in notes.csv for NLP crosswalk and language-audit teaching activities.

The package avoids direct identifiers and does not contain PHI.
Synthetic IDs are internally linkable across files via patient_id, and notes can link to encounters via encounter_id. Hosting for Google Colab Option A: GitHub raw URLs

Suggested notebook URL mapping Notebook Dataset URL to use

Module 4 NLP data/notes.csv Module 5 Visualization data/post_overdose_data.csv Module 6 Machine Learning data/hopebridge_ml.csv Module 7 Deep Learning & Images no CSV required for template; optional use of data/encounters.csv for reflection metadata Module 8 Capstone all CSVs as optional integrated evidence sources

Stigma-free language reference Use person-first language such as "person with opioid use disorder," "person with a substance use disorder," "substance use," "positive toxicology result," and "negative toxicology result." Avoid terms such as "addict," "drug abuser," and "clean/dirty" for toxicology results. See NIDA's Words Matter guidance: https://nida.nih.gov/nidamed-medical-health-professionals/health-professions-education/words-matter-terms-to-use-avoid-when-talking-about-addiction

Files
[Open In Colab] (https://colab.research.google.com/github/USERNAME/REPOSITORY/blob/main/notebooks/WISER_M4.ipynb)
