# Hydration free energy of small molecules in water

Estimates the free energy released when a small molecule is transferred from vacuum into water, a quantity that underpins how tightly a solvated ligand can be pulled into a binding site. Training used FreeSolv, the MoleculeNet set of 642 molecules pairing experimental hydration free energies with alchemical calculations. A graph transformer pretrained without labels on 10 million ChEMBL and ZINC15 molecules was fine-tuned on it, averaging three folds per prediction. FreeSolv is small and dominated by neutral organic compounds, so charged or unusual chemistry sits outside its range.

This model was incorporated on 2022-07-13.
Last packaged on 2026-11-03.

## Information
### Identifiers
- **Ersilia Identifier:** `eos157v`
- **Slug:** `grover-freesolv`

### Domain
- **Task:** `Annotation`
- **Subtask:** `Property calculation or prediction`
- **Biomedical Area:** `ADMET`
- **Target Organism:** `Any`
- **Tags:** `MoleculeNet`, `Chemical graph model`, `Quantum properties`

### Input
- **Input:** `Compound`
- **Input Dimension:** `1`

### Output
- **Output Dimension:** `1`
- **Output Consistency:** `Fixed`
- **Interpretation:** Hydration free energy in kcal/mol, where more negative values indicate stronger solvation.

Below are the **Output Columns** of the model:
| Name | Type | Direction | Description |
|------|------|-----------|-------------|
| freesolv | float | low | Hydration free energy in kcal/mol |


### Source and Deployment
- **Source:** `Local`
- **Source Type:** `External`
- **DockerHub**: [https://hub.docker.com/r/ersiliaos/eos157v](https://hub.docker.com/r/ersiliaos/eos157v)
- **Docker Architecture:** `AMD64`, `ARM64`
- **S3 Storage**: [https://ersilia-models-zipped.s3.eu-central-1.amazonaws.com/eos157v.zip](https://ersilia-models-zipped.s3.eu-central-1.amazonaws.com/eos157v.zip)

### Resource Consumption
- **Model Size (Mb):** `1292`
- **Environment Size (Mb):** `2406`
- **Image Size (Mb):** `3669.8`

**Computational Performance (seconds):**
- 10 inputs: `28.03`
- 100 inputs: `97.74`
- 10000 inputs: `-1`

### References
- **Source Code**: [https://github.com/tencent-ailab/grover](https://github.com/tencent-ailab/grover)
- **Publication**: [https://doi.org/10.48550/arXiv.2007.02835](https://doi.org/10.48550/arXiv.2007.02835)
- **Publication Type:** `Preprint`
- **Publication Year:** `2020`
- **Ersilia Contributor:** [Amna-28](https://github.com/Amna-28)

### License
This package is licensed under a [GPL-3.0](https://github.com/ersilia-os/ersilia/blob/master/LICENSE) license. The model contained within this package is licensed under a [MIT](LICENSE) license.

**Notice**: Ersilia grants access to models _as is_, directly from the original authors, please refer to the original code repository and/or publication if you use the model in your research.


## Use
To use this model locally, you need to have the [Ersilia CLI](https://github.com/ersilia-os/ersilia) installed.
The model can be **fetched** using the following command:
```bash
# fetch model from the Ersilia Model Hub
ersilia fetch eos157v
```
Then, you can **serve**, **run** and **close** the model as follows:
```bash
# serve the model
ersilia serve eos157v
# generate an example file
ersilia example -n 3 -f my_input.csv
# run the model
ersilia run -i my_input.csv -o my_output.csv
# close the model
ersilia close
```

## About Ersilia
The [Ersilia Open Source Initiative](https://ersilia.io) is a tech non-profit organization fueling sustainable research in the Global South.
Please [cite](https://github.com/ersilia-os/ersilia/blob/master/CITATION.cff) the Ersilia Model Hub if you've found this model to be useful. Always [let us know](https://github.com/ersilia-os/ersilia/issues) if you experience any issues while trying to run it.
If you want to contribute to our mission, consider [donating](https://www.ersilia.io/donate) to Ersilia!
