# Latex Formatting of my PhD dissertation

2022-02-23

This is the dissertation template for My PhD. Feel free to use.

<!-- TOC -->

- [Latex Formatting of my PhD dissertation](#latex-formatting-of-my-phd-dissertation)
  - [How to make label and ref consistent](#how-to-make-label-and-ref-consistent)
  - [Compile issues (When using Tex Shop)](#compile-issues-when-using-tex-shop)
  - [Dissertation requirements](#dissertation-requirements)

<!-- /TOC -->
## How to make label and ref consistent

find and replace all label and ref by adding prefix `chp[num]-`. Use non-greedy `?`.

**in chp1.tex do**  

```python
\\label\{(.*?)\} #find
\\label{chp1-$1} #replace

\\ref\{(.*?)\} #find
\\ref{chp1-$1} #replace
```

## Compile issues (When using Tex Shop)

try xelatex->bibtex->xelatex->xelatex

>better to use the extension [LaTeX-Workshop](https://github.com/James-Yu/LaTeX-Workshop) in vscode

## Dissertation requirements

- [x] Abstract: The body of the abstract may not exceed 350 words in length.
- [x] Minimum Margins: The minimum acceptable margins for all pages of the dissertation and the abstract are 1 inch on left and 1 inch on the top, bottom, and right.
- [x] Font and Point Size: Recommended fonts include Arial, **Times New Roman**, and Helvetica with a point size of either 11 or **12**.
- [x] Print: Print should be clear, clean, and dark with no shadows or stray marks.  Remember to remove tracking changes.
- [x] Spacing: The text of the dissertation should be double-spaced. Long quotations, footnotes, appendices, and references may be single-spaced.
- [x] Photographs and Graphics: Photographs, graphics, and scanned images in the dissertation should be high quality. The use of color is acceptable.
- [x] Use of materials copyrighted by others: Any material included that goes beyond “fair use” requires written permission of the copyright owner. See specifications on Submittable. It may be useful to include these in the dissertation as an appendix.
- [x] Pagination: Preliminary pages (the title page, optional copyright page, acknowledgments, table of contents, and the like) are to be numbered consecutively using lower case Roman numerals.  The title page number may be suppressed. All pages of the text, appendices (if any), and references must be numbered consecutively using Arabic numerals. The abstract is not paginated. Page number locations should be consistent throughout the document.
- [x] Landscape pages: The top of a landscape page should be at the left margin and the bottom at the right margin. The page number is to be in the same relative position as on the portrait pages.
- [x] Sequence of the main components of the dissertation: The appropriate order of the major sections of the dissertation follows:   

```mermaid
flowchart LR;
  abstract --> title --> copyright--> committee--> acknowledgments;
  acknowledgments--> TOC--> Main--> references--> appendices;
```
The order of the appendices and the references may be reversed if the appendices are lengthy.
- [x] Footnotes, Endnotes, and References: The format that is accepted in your discipline or that is prescribed by your advisory committee should be followed.
- [x] Photocopied journal articles in the dissertation: When appropriate, photocopied articles already published in journals may be included in a dissertation. Photocopying must conform to the margins noted above. An original letter from each journal, granting permission for the inclusion of the photocopied article in the dissertation is necessary to assure that there are no permission issues or violations of copyright. In requesting a letter of permission, it is important to tell the journal that Submittable will be posting the dissertation to third party search engines. The journal usually will require that the journal be the first publisher of the article. Please retain a copy of all permissions granted for your personal file.