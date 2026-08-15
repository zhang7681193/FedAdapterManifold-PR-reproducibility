# FedAdapterManifold reproducibility package

This repository contains the public research-data and reproducibility package for the Pattern Recognition manuscript:

**FedAdapterManifold: Deciding When Federated Visual LoRA Adapters Are Safe to Share**

The package supports the paper's central claim that federated visual LoRA adapters should not be treated as globally averageable vectors: adapter subspace incompatibility predicts FedAvg-LoRA aggregation failure, and geometry-conditioned anchored routing can reduce negative transfer under heterogeneous visual recognition settings.

## Repository contents

- `reproducibility/FedAdapterManifold_Reproducibility_Package.zip`  
  Clean reproducibility archive containing code, YAML configs, plotting scripts, audited result summaries, figures, reports, and manuscript-linked experiment artifacts.
- `MANIFEST.md`  
  Human-readable description of the archive contents, expected use, and checksum.
- `CITATION.cff`  
  Citation metadata for the reproducibility package.
- `LICENSE`  
  Repository license for the released code/data package.

## Archive checksum

File: `reproducibility/FedAdapterManifold_Reproducibility_Package.zip`

SHA256:

```text
5F9E4A66416D26A01CCA24AD9873BB1BC5F950BFB232DE630DC0EC879AA31D11
```

Size: 3,392,879 bytes.

## What is included

The archive includes:

- experiment runner scripts and reusable Python modules;
- YAML configuration files for the audited settings;
- per-seed and aggregate result CSVs used by the manuscript;
- figure-generation scripts and figure assets;
- subspace diagnostic, adapter conflict, routing, and VFM/backbone audit summaries;
- fixed candidate-pool, calibration-split, baseline-fidelity, and no-oracle audits;
- the untouched OfficeHome confirmation summaries for seeds 10--14;
- the training-only conditional `FAM|Geo` audit used to isolate the incremental
  adapter-subspace contribution; and
- a reproducibility README with expected execution notes.

The large frozen geometry payload is distributed separately from this compact
archive. The compact package contains its registries, hashes, manifests, and
validation reports, but not external benchmark images.

The archive does **not** redistribute external benchmark datasets. Users should obtain datasets such as PACS, OfficeHome, DomainNet, and MedMNIST from their official sources and follow their respective licenses.

## Research data metadata for submission systems

- Repository name: GitHub
- Source of data: Original data
- Dataset title: FedAdapterManifold reproducibility package and experimental results
- URL: https://github.com/zhang7681193/FedAdapterManifold-PR-reproducibility

## Contact

For questions about this reproducibility package, please contact the corresponding author listed in the manuscript.
