# OSCAL

This repo provides the Monetary Authority of Singapore (MAS) Notice of Cyber Hygiene in the Open Security Controls Assessment Language (OSCAL), a standardised machine-readable format by the US NIST. This notice is provided as an OSCAL catalog with a corresponding OSCAL profile - useful for building automated system security plans (SSPs) and embedding into CI automation jobs. 

## Validation

You can validate that the catalog is in a valid OSCAL format as declared in the documents metadata field using [https://github.com/defenseunicorns/go-oscal/](go-oscal).

```
./go-oscal validate -f mas_cyber_hygiene_catalog.yaml
```

