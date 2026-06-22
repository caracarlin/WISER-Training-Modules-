WISER Colab Notebook Templates for Modules 4–8
This package contains starter Google Colab notebooks for the WISER course modules:

notebooks/WISER_M4_NLP_Semantics_Template.ipynb
notebooks/WISER_M5_Data_Visualization_Template.ipynb
notebooks/WISER_M6_Machine_Learning_Template.ipynb
notebooks/WISER_M7_Deep_Learning_Images_Template.ipynb
notebooks/WISER_M8_Capstone_Integration_Template.ipynb
How to publish
Upload this folder to a GitHub repository or Google Drive.

Replace blank DATA_URL values with stable URLs for the final WISER synthetic datasets.

Open each notebook in Google Colab.

Run Runtime → Restart and run all.

Fix any dependency or data-loading issues.

In Articulate Rise, add a button block labeled Open Google Colab Notebook.

If using GitHub, link each notebook with:

https://colab.research.google.com/github/YOUR-ORG/YOUR-REPO/blob/main/notebooks/NOTEBOOK_NAME.ipynb
Design notes

Each notebook includes synthetic fallback data so instructors can test without external files.
Each notebook has Foundational and Applied pathway sections in the same file.
Each notebook exports a small FAIR-oriented outputs/metadata.json and outputs/README.md.
Learners are instructed not to upload PHI or identifiable institutional data.
Stigma-free terminology helper functions are included in every notebook.
Recommended validation
Before release, run every notebook from a clean runtime and confirm:

No hidden local paths remain.
All outputs are generated.
All charts have alt text prompts.
All data are synthetic, public, or instructor-approved.
No paid API key or paid software is required.
