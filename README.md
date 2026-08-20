README.md
#!/bin/bash

RECEPTOR="input/receptor.pdbqt"
LIGAND="input/ligand.pdbqt"
OUTPUT="output/docked_poses.sdf"
LOG="output/docking_log.txt"

echo "Running GNINA molecular docking..."

gnina \
  --receptor $RECEPTOR \
  --ligand $LIGAND \
  --autobox_ligand $LIGAND \
  --out $OUTPUT \
  --log $LOG \
  --exhaustiveness 8 \
  --cpu 4

echo "Docking completed successfully!"
