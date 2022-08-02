# Name badges and participation certificates for Brainhack events

This repository contains the tools to create name badges and participation
certificates for Brainhack events.

A `.csv` file containing the names and affiliations of event attendees is
required to make the badges and certificates.

## Making name cards and certificates for your event

1. Create a `.csv` containing names and affiliations for your attendees. See
[`example_namelist.csv`](data/namelist/example_namelist.csv) for an example.
2. Modify [`template_id_cards.tex`](template_id_cards.tex) and 
[`template_certificate.tex`](template_certificate.tex) to fit your event.
to reflect your event information and the filename of your participant list.
3. [`template_certificate.tex`](template_certificate.tex) will
additionally need to modified to contain the name of the local event chair, and
a `PDF` of their signature. Note that the **current signature** in the
[`data/signature`](data/signature) folder is a **mock signature** and **does not
and cannot be accounted for anyone's signature or endorsement**.
4. Compile the cards and certificates into a `PDF` using `pdflatex`, for
example:

```bash
pdflatex template_certificate.tex
```
or
```bash
pdflatex template_id_cards.tex
```

You can upload the files to `Sharelatex` or `Overleaf` and compile them there
or install `LaTeX` on your local system.
