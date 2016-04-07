# Newcastle Computing Science PhD Template LaTeX
This guide is intended for students in the [School of Computing Science](www.cs.ncl.ac.uk) at Newcastle University.


## Starting point
CUED LaTeX template by Krishna Kumar at https://github.com/kks32/phd-thesis-template.

## Custom margins

To add custom margins, in accordance with the guidelines, 

```` \documentclass[a4paper,12pt,times,numbered,print,index]{Classes/PhDThesisPSnPDF} ````

```` \documentclass[a4paper,12pt,times,numbered,print,index,custommargin]{Classes/PhDThesisPSnPDF} ````


In your ```` Preamble/Preamble.tex````, set the custom margin as follows:

```` 
% Add `custommargin' in the document class options to use this section
% Set {innerside margin / outerside margin / topmargin / bottom margin}  and
% other page dimensions
\ifsetCustomMargin
  \RequirePackage[left=30mm,right=20mm,top=20mm,bottom=20mm]{geometry}
  \setFancyHdr % To apply fancy header after geometry package is loaded
\fi
````
