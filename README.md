# NS-ID — Neuro-Symbolic Integral Derivator

**Project status:** research project / implementation documentation in progress.

NS-ID explores a neuro-symbolic approach to reading handwritten integral expressions and producing mathematically verified symbolic solutions.

## Research goal

Handwritten mathematics recognition is challenging because expressions contain two-dimensional structure, ambiguous symbols and notation that cannot always be represented reliably as ordinary text.

The project aims to combine a vision-language model with symbolic mathematics tools so that visual recognition and mathematical validation support one another.

## Intended pipeline

1. **Image input:** receive a photograph or scan of a handwritten integral.
2. **Visual understanding:** recognize mathematical symbols and their spatial relationships.
3. **Expression reconstruction:** convert the recognized expression into a structured mathematical representation.
4. **Symbolic processing:** use SymPy to parse, differentiate or integrate the expression where supported.
5. **Verification:** check the proposed antiderivative by differentiating it and comparing it with the input integrand.
6. **Presentation:** return the reconstructed expression, solution and verification status.

## Research directions

- Vision-language models for handwritten mathematical expression recognition.
- Mathematical structure and LaTeX reconstruction.
- Neuro-symbolic correction and constraint-based validation.
- Evaluation on handwritten-integral examples and public mathematical expression datasets.

## Repository contents

At the moment, this repository contains this project README only. The model code, data-processing pipeline, evaluation scripts and reproducible experiments still need to be added before the implementation can be independently reproduced.

## Planned structure

```text
NS_ID/
├── data/              # Dataset instructions and split definitions
├── notebooks/         # Exploration and experiments
├── src/
│   ├── recognition/   # Image-to-expression model
│   ├── symbolic/      # SymPy parsing and verification
│   └── evaluation/    # Metrics and error analysis
├── examples/          # Handwritten inputs and expected outputs
├── requirements.txt
└── README.md
```

## Tech direction

Python · Vision-Language Models · LaTeX · SymPy · PyTorch

## Reproducibility

This is a research direction, not yet a reproducible release. Model names, datasets, training configuration and benchmark results will be documented here once they are committed to the repository.

## License

No license is currently specified. Contact the repository owner before reuse.
