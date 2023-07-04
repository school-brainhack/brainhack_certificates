# Name badges and participation certificates for Brainhack School

This repository contains the tools to create name badges and participation
certificates for Brainhack School.

A `CSV` file containing the names and affiliations of event attendees is
required to make the badges and certificates.

## Making name cards and certificates for your hub

1. Create a `CSV`containing names and affiliations for your attendees. See
[`example_namelist.csv`](data/namelist/example_namelist.csv) for an example.
2. Modify [`brainhack_school_id_cards.tex`](latex/brainhack_school_id_cards.tex).
3. For the graduation certifications we have two template. If you plan to have 
signatures of the organizers, please use [`brainhack_school_certificate_signature.tex`](
latex/latex/brainhack_school_certificate_signature.tex). 
If you only list the logos of the sponsors, please use the if you to reflect your event information [`brainhack_school_certificate_logos.tex`](
latex/latex/brainhack_school_certificate_logos.tex) and the filename of your participant list.
4. The certificate tex files will need to  be modified the name of the hub organizer(s) and hub details.
5. If you plan to use a signature from an image or pdf file, then uncomment the line that reads the signature file under signature folder. 
**Note that the current signature in the data/signature folder is a mock signature and does not and cannot be accounted for anyone's signature or endorsement.**
6. Compile the cards and certificates into a `PDF` using `pdflatex`, for example:

```bash
pdflatex examples/brainhack_school_id_cards.tex
```
or
```bash
pdflatex examples/brainhack_school_UdeM_certificate.tex
```

You can upload the files to `Sharelatex` or `Overleaf` and compile them there
or install `LaTeX` on your local system.
