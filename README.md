# 🧬 Docking Analysis: Phosphorylcholine (PC) with Human OLR1

## Research Aim
To study the docking interaction between PC and OLR1, providing insights into cardiovascular disease (CVD) mechanisms.

## Background
Phosphorylcholine (PC) is a small molecule composed of a negatively charged phosphate bonded to a positively charged choline group.  
- Found in both prokaryotes and eukaryotes.  
- Plays a role in bacterial cell walls (e.g., *Streptococcus pneumoniae*, *Haemophilus influenzae*).  
- Used in biomaterials (drug‑eluting stents, contact lenses) due to its biocompatibility.  
- Molecular weight: 183.14 g/mol  
- Formula: C5H14NO4P  

## OLR1 Gene
The OLR1 gene encodes a receptor for oxidized low‑density lipoprotein (oxLDL).  
- Belongs to the C‑type lectin superfamily.  
- Regulated through cyclic AMP signaling.  
- Functions: binds, internalizes, and degrades oxLDL.  
- Biological roles: scavenger receptor activity, regulation of Fas‑induced apoptosis.  
- Clinical relevance: mutations linked to atherosclerosis, myocardial infarction risk, and potentially Alzheimer’s disease.

## 🔍 Problem Statement
Exploring the binding interaction between **Phosphorylcholine (PC)** and the **human OLR1 receptor (oxidized low-density lipoprotein receptor 1)**, a key player in cardiovascular disease (CVD).

## 🌍 Importance
OLR1 is linked to atherosclerosis, myocardial infarction, and Alzheimer’s disease risk. Understanding PC–OLR1 binding may reveal molecular mechanisms of vascular inflammation and lipid metabolism, offering potential therapeutic insights.

## 📊 Data Used
- **Ligand**: Phosphorylcholine (PubChem CID: 135437)  
- **Protein**: OLR1 receptor (PDB ID: 1YPQ)  
- **Active site**: Docking focused around residue **PHE158**

## ⚙️ Methodology
1. **Protein & Ligand Preparation**  
   - Removed water molecules  
   - Added polar hydrogens  
   - Applied Kollman charges  
   - Saved in PDBQT format  

2. **Docking Setup**  
   - Grid box spacing: 0.375 Å  
   - Dimensions: 58 × 56 × 56 (X, Y, Z)  
   - Center coordinates: (11.434, 3.915, 19.020)  
   - Energy range: 4  
   - Exhaustiveness: 8  

3. **Docking Execution**  
   - AutoDock Vina with config file specifying protein, ligand, and grid parameters  

# 📈 Docking Results: PC with OLR1

## Grid Box Parameters
- Spacing: 0.375 Å  
- Dimensions: 58 × 56 × 56 (X, Y, Z)  
- Center coordinates: (11.434, 3.915, 19.020)  
- Energy range: 4  
- Exhaustiveness: 8  

## Binding Affinities
The docking predicted multiple binding modes. The best mode had the strongest affinity.

| Mode | Affinity (kcal/mol) | RMSD l.b. | RMSD u.b. |
|------|---------------------|-----------|-----------|
| 1    | -4.2               | 0.000     | 0.000     |
| 2    | -3.9               | 1.196     | 2.294     |
| 3    | -3.8               | 3.485     | 5.006     |
| 4    | -3.5               | 45.353    | 46.289    |
| 5    | -3.5               | 1.725     | 2.540     |

## Key Observations
- Best binding affinity: **-4.2 kcal/mol**.  
- RMSD values confirm stable binding (<2 Å for best mode).  
- Multiple alternative poses with slightly weaker affinities (-3.9 to -3.5 kcal/mol).  

## Interpretation
The docking suggests that PC can bind to OLR1 with moderate affinity, potentially influencing receptor activity and oxLDL uptake.

# 🧬 Discussion: Biological Implications of PC–OLR1 Docking

## Structural Insights
- Removal of water molecules improved electrostatic accuracy.  
- Addition of polar hydrogens and Kollman charges ensured reliable binding affinity predictions.  
- Docking centered around residue PHE158, a key active site in OLR1.

## Biological Meaning
- PC binding to OLR1 may modulate receptor activity.  
- Since OLR1 regulates oxLDL uptake, this interaction could influence lipid metabolism and vascular inflammation.  
- Supports the hypothesis that PC contributes to **atherosclerosis progression** and **cardiovascular disease risk modulation**.

## Future Directions
- Experimental validation of PC–OLR1 binding through wet‑lab assays.  
- Investigation of binding effects on downstream signaling pathways.  
- Potential exploration of PC analogs as therapeutic modulators of OLR1.
