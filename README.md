# uspto-chem

USPTO Chemical Compounds Extraction

Extracted chemical compounds from USPTO .CDX attachments since 2001 using RDKit.

Each week, the USPTO uploads two tar files: one for patent grants (Tuesday) and one for patent applications (Thursday). For each of the files, patents are filtered by IPC/CPC codes relevant to the pharmaceutical sector, first, patent metadata is extracted; then every .CDX attachment is located and compounds are extracted alongside the metadata. Each USPTO tar file produces a corresponding JSON file with the extracted data. Compounds are parsed and saved as CXSMILES with RDKit.
Focus IPC/CPC classes

    C07 — Organic chemistry (Section C: Chemistry). Covers organic compounds and their synthesis, including heterocycles, sugars, peptides, etc.
    A61K — Preparations for medical, dental, or toilet purposes (Section A: Human necessities). Pharmaceutical compositions/formulations and ingredient categories.
    A61P — Specific therapeutic activity of chemical compounds or medicinal preparations. Indicates the medical indication (e.g., analgesic, antineoplastic); pairs with A61K.
    A01N — Preservation of bodies; biocides (disinfectants, pesticides, herbicides), pest control, and plant growth regulators (Section A: Agriculture/human necessities). Focuses on active agents and uses in these domains.


https://eloyfelix.github.io/uspto-chem/