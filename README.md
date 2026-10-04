# Global AI Risk Observatory

We measure how companies write about artificial intelligence in their regulatory filings: whether AI appears as a technology they use, a product they sell, a market they depend on, or a risk they carry, and how specifically they say so.

The data are audited, legally mandated corporate reports. They are published on a fixed schedule in a regulated context, which makes them a reliable baseline for tracking corporate AI exposure at scale, unlike surveys or voluntary disclosures.

## Scope

The first phase covers US filings (Form 10-K and related SEC forms). Other jurisdictions follow once the US pipeline is validated. The target scale is several hundred thousand reports.

## How it works

1. Filings are collected and parsed into text blocks with their report section.
2. Candidate passages are found with a core AI vocabulary plus industry-specific glossaries (one per ISIC Rev. 5 division). Passages that name AI go to classification; passages that only touch AI-linked topics are kept as hints for a reader.
3. Each passage is labelled against a published codebook: frame, role of AI, risk type, adoption stage, kind of AI, disclosure traits, named entities, verbatim evidence.
4. Several independent coders, human and model, label the same passages; labels are reconciled by majority vote and agreement is reported.
5. Results are aggregated per report, year and industry.

The taxonomy is versioned; every change is recorded with what it replaced and why.

## Status

Early. The pipeline runs end to end on single filings; the codebook is at version 0.4; human annotation and the first large-scale run are being prepared. Research questions are being defined with the policy team and are not final.

## Repositories

- `classification-pipeline`: the pipeline, glossaries, codebook, research plan and change log.

## Working with us

Issues and pull requests in the repositories above. Report data cannot be redistributed; the repositories contain code, glossaries and derived labels only.
