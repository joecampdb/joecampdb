<div align="center">

# Hey, I'm JoeCamPDB 👋

**Structural bioinformatics · AI for TechBio · molecular simulation**

<br>

<img src="https://raw.githubusercontent.com/joecampdb/joecampdb/main/knot_writhe_ssfm_vs_painn.gif" alt="Ray-marched animation of a knotted trefoil polymer rolled out by two learned surrogates. The SSFM-style stepper holds the knot while the PaiNN-style stepper unties it, shown by the writhe traces below." width="100%">

<sub>**A knot is a metric your structural scores can't see.** Same trefoil, two learned surrogates,
ray-marched as SDF tubes with soft self-shadows. The SSFM-style stepper (green) tracks reference writhe at |w| ≈ 3.5
for the whole rollout; the PaiNN-style stepper (red) drifts toward 0 — the ring has passed
through itself and the trefoil is gone.</sub>

</div>

I'm a bioinformatics researcher specializing in structural biology, with a focus on developing
robust, reusable tooling and scaffolding for protein structure prediction, design, and analysis
using modern AI techniques (e.g. geometric deep learning).

While I maintain interest in genomics and transcriptomics, my primary efforts are now centered on
structural bioinformatics, co-folding algorithms, and related AI methods.

---

## Selected work

### 🪢 Does the surrogate keep the knot?
**Topology preservation in learned polymer-dynamics models**

Learned surrogates for molecular dynamics are graded on *structure* (radius of gyration, contacts)
and *dynamics* (diffusion, relaxation). This project asks a third question those metrics can miss
entirely: **when a surrogate rolls out a knotted polymer, does the knot survive?**

On a controlled ladder of coarse-grained Kremer–Grest systems, the model with the **best**
structural score (Rg-W2 = 0.02) retains the trefoil in only **49%** of frames — the ring breaks and
collapses into a compact tangle that still *looks* right structurally. Only a topology metric
exposes it. The stable steppers keep the knot **100%** of the time, with no topology conditioning
at all.

> Stability — not expressivity, not topology-conditioning — is what preserves topology.

### 🧫 MEM-CALVADOS membrane pipeline
**Coarse-grained membranes, from force field to ray-traced frame**

End-to-end simulation and analysis for coarse-grained bilayers and vesicles: curvature and
electrostatics analysis, HCN1 in a membrane environment, vesicle systems up to 35 nm, and an
OVITO/Tachyon rendering path that turns trajectories into publication frames.

### 🧬 DNA origami nanoswitches
**Characterizing the bond angle distribution of DNA origami nanoswitches — master's thesis, 2025**

Scaffold extensions on a DNA origami nanoswitch, built in oxView and simulated with the oxDNA2
force field in LAMMPS. The thesis went after one mechanical property of these devices: how the
**bond angle distribution** across a flexible linker responds to linker length.

The obvious hypothesis is that a longer linker buys more conformational freedom. It doesn't.
Across linkers of 10, 20, 30 and 40 nucleotides, angular variance *falls* as the linker grows,
decaying exponentially — longer linkers **stabilize** the joint rather than loosening it.

https://github.com/user-attachments/assets/919276d8-6a91-46fc-bdd3-2cc9d2bb8c4b

---

## About me

- Background in structural biology, materials science, computational epigenetics, and neuroscience.
- Passionate about understanding systems at molecular, biological, and computational levels.
- 🌱 Currently learning geometric deep learning, manifold learning, and advanced docking / side-chain packing.
- 🤔 Seeking collaboration on persistent homology and optimization challenges in protein modeling.
- 💬 Ask me about protein folding algorithms, geometric deep learning on biomolecules, or AlphaFold variants.
- ⚡ Fun fact: humans are about one centimeter taller in the morning than at night, from spinal disc decompression.

## Toolkit

**Structure prediction & design**

![AlphaFold](https://img.shields.io/badge/AlphaFold-4285F4?style=flat-square&logo=google&logoColor=white)
![ColabFold](https://img.shields.io/badge/ColabFold-FF9900?style=flat-square&logo=jupyter&logoColor=white)
![Boltz-2](https://img.shields.io/badge/Boltz--2-4A90E2?style=flat-square)
![ProteinMPNN](https://img.shields.io/badge/ProteinMPNN-6A1B9A?style=flat-square)
![DiffDock](https://img.shields.io/badge/DiffDock-7E57C2?style=flat-square)
![AutoDock](https://img.shields.io/badge/AutoDock-388E3C?style=flat-square)

**Geometric deep learning**

![PyTorch Geometric](https://img.shields.io/badge/PyTorch%20Geometric-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![e3nn](https://img.shields.io/badge/e3nn-0769AD?style=flat-square&logo=python&logoColor=white)
![CUDA](https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white)

**Simulation**

![GROMACS](https://img.shields.io/badge/GROMACS-1565C0?style=flat-square)
![OpenMM](https://img.shields.io/badge/OpenMM-005571?style=flat-square)
![LAMMPS](https://img.shields.io/badge/LAMMPS-0277BD?style=flat-square)
![oxDNA](https://img.shields.io/badge/oxDNA-2E7D32?style=flat-square)
![MDAnalysis](https://img.shields.io/badge/MDAnalysis-FF6F00?style=flat-square)

---

<div align="center">

📫 **[joecamxtc@gmail.com](mailto:joecamxtc@gmail.com)** &nbsp;·&nbsp; 𝕏 **[@bioinfojoe](https://x.com/bioinfojoe)** &nbsp;·&nbsp; he/him

<sub>Several repositories are private while the work is in progress.</sub>

</div>
