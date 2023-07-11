# Hydration free energy of small molecules in water

Model based on experimental and calculated hydration free energy of small molecules in water, the FreeSolv dataset from MoleculeNet. Hydration free energies are relevant to understand the binding interaction between a molecule (in solution) into its binding site.  This model has been trained using the GROVER transformer (see eos7w6n or grover-embedding for a detail of the molecular featurization step with GROVER). 

## Identifiers

* EOS model ID: `eos157v`
* Slug: `grover-freesolv`

## Characteristics

* Input: `Compound`
* Input Shape: `Single`
* Task: `Regression`
* Output: `Other value`
* Output Type: `Float`
* Output Shape: `Single`
* Interpretation: Calculated Hydration Free energy in kcal/mol

## References

* [Publication](https://papers.nips.cc/paper/2020/hash/94aef38441efa3380a3bed3faf1f9d5d-Abstract.html)
* [Source Code](https://github.com/tencent-ailab/grover)
* Ersilia contributor: [Amna-28](https://github.com/Amna-28)

## Ersilia model URLs
* [GitHub](https://github.com/ersilia-os/eos157v)

## Citation

If you use this model, please cite the [original authors](https://papers.nips.cc/paper/2020/hash/94aef38441efa3380a3bed3faf1f9d5d-Abstract.html) of the model and the [Ersilia Model Hub](https://github.com/ersilia-os/ersilia/blob/master/CITATION.cff).

## License

This package is licensed under a GPL-3.0 license. The model contained within this package is licensed under a MIT license.

Notice: Ersilia grants access to these models 'as is' provided by the original authors, please refer to the original code repository and/or publication if you use the model in your research.

## About Us

The [Ersilia Open Source Initiative](https://ersilia.io) is a Non Profit Organization ([1192266](https://register-of-charities.charitycommission.gov.uk/charity-search/-/charity-details/5170657/full-print)) with the mission is to equip labs, universities and clinics in LMIC with AI/ML tools for infectious disease research.

[Help us](https://www.ersilia.io/donate) achieve our mission!