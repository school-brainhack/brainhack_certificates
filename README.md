# Name badges and participation certificates for Brainhack School

This repository contains the tools to create name badges and participation
certificates for Brainhack School.

A `CSV` file containing the names and affiliations of event attendees is
required to make the badges and certificates.

## Making name cards and certificates for your hub

1. Create a `CSV`containing names and affiliations for your attendees. See
[`example_namelist.csv`](data/namelist/example_namelist.csv) for an example.
2. Modify [`brainhack_school_id_cards.tex`](latex/brainhack_school_id_cards.tex) and [`brainhack_school_certificate.tex`](
latex/latex/brainhack_school_certificate.tex) to reflect your event information and
the filename of your participant list.
3. [`brainhack_school_certificate.tex`](latex/brainhack_school_certificate.tex) will
additionally need to modified to contain the name of the hub organizers, and
a `PDF` of their signature. Note that the **current signature** in the
[`data/signature`](data/signature) folder is a **mock signature** and **does not
and cannot be accounted for anyone's signature or endorsement**.
1. Compile the cards and certificates into a `PDF` using `pdflatex`, for
example:

```bash
pdflatex examples/brainhack_school_id_cards.tex
```
or
```bash
pdflatex examples/brainhack_school_UdeM_certificate.tex
```

You can upload the files to `Sharelatex` or `Overleaf` and compile them there
or install `LaTeX` on your local system.
