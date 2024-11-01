# KNIME workflows for chemoinformatic characterization of chemical databases
This repository contains KNIME workflows for chemical database characterization: including descriptor calculation, Bemis-Murcko scaffold identification, PAINS detection, MACCS fingerprint calculation, and visual representation of chemical space based on fingerprints. 

The workflows compiled include various types of nodes. The initial node is a reader-type node, which extracts information from a source document. This source document contains a column with chemical representations and its format could be varied such as CSV, table, XLSX, or SDF.

The next node is a converter-type node that transforms the dataset from a string format into a chemical representation, such as SMILES, SMARTS, InChiKeys, etc. 

The third node converts the linear notation into a specific object, which is then used by the subsequent node to perform various chemoinformatic analyses: Calculation of descriptors and molecular fingerprints, and identification of substructures like PAINS and molecular scaffolds. Due to this node's different calculations, it will be referred to as an action node. 

Finally, a writer-type node must be added, so the results can be stored. Sometimes, a visualization-type node can also be added (necessary when data visualization is needed such as the visual representation of chemical space).


Feel free to download the workflows to perform your own chemical database characterization.
