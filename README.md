Purpose

It’s an interactive web form for collecting structured information about organoid-on-chip experiments — so that biologists can describe their experimental setup in a way that’s compatible with your ontology-driven digital twin project.

Essentially, it bridges wet-lab metadata and in-silico models.

🧠 Main Functions
1. Data collection

The form covers (in the full version):

Administrative info: project ID, species, tissue, disease, etc.

Experimental design: chip geometry, ECM, flow, oxygen, temperature.

Cell composition: proportions of tumor, fibroblast, immune cells, etc.

Stimuli: drugs, cytokines, dosages, and timing.

Readouts: omics, imaging, viability, etc.

Narrative section: free-text notes and observations.

All fields are structured to map to ontology terms (e.g., MONDO, UBERON, CL, ChEBI).

2. JSON export

When you click Export JSON, the form:

Gathers all filled fields into a machine-readable .json file.

Uses a consistent schema (keys like cell_fractions.tumor, oxygen.setpoint_percent, etc.).

This JSON can feed directly into your digital twin pipeline or be parsed for ontology population.

3. Graphviz DOT generation

Click Generate DOT graphs and the form will:

Create two .dot files (for Graphviz visualization):

In-vivo vs. Experiment Graph — shows which biological nodes (tumor, fibroblast, VEGF, hypoxia, etc.) are represented in your experiment versus missing in the real system.

Difference Graph — highlights what’s absent in the experiment compared to the full in-vivo model.

These graphs visually represent how close the experiment is to physiological reality — your “distance metric” in the ontology space.

4. Demo + Reset

A Demo Fill button (in the full version) auto-populates an example setup so you can test exports.

Clear resets all fields instantly.
