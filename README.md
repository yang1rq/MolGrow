# MolGrow
### A digital fragment-growing method accelerates the discovery of agricultural fungicides

## Requirements
```
torch        1.13.1
dgl-lifesci  0.3.2
rdkit        2022.9.5
openbabel    3.1.1
vina         1.2.7
```

## Usage
### If you want to use DigGrow to generate molecules in a fragment-based manner based on the given target protein, run the command:
```
python main.pyc
```

### Model parameter configuration
```
--ligand: "Ligand (.sdf) to determine the position of pocket"
--protein: "Target protein (.pdbqt)"
--start: "Start fragment (.sdf)"
--frag_lib: "Fragment library (.txt)"
--attentivefp: "Model weights for predicting substitution sites (.pth)"
--vina: "Molecular docking executable file (.exe)"
--num_mols: "The maximum number of generated molecules"
--frag_count: "The threshold for fragment count"
--mol_weight: "The threshold for molecular weight"
--max_force: "The threshold for maximum force"
```

Please note that the "building blocks" code is sourced from [Du et al](https://github.com/Brian-hongyan/3D-MCTS).

### If you have any questions, please contact Fan Wang (fwang@ccnu.edu.cn) or Guangfu Yang (gfyang@ccnu.edu.cn)
