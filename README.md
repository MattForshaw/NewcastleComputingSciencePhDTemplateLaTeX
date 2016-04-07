# Newcastle Computing Science PhD Template LaTeX
This guide is intended for students in the [School of Computing Science](www.cs.ncl.ac.uk) at Newcastle University.

This is particularly targetted at PhD students required to conform to _Guidelines for the Submission and Format of Theses_ ([April 2015 version](http://www.ncl.ac.uk/students/progress/assets/documents/GuidelinesfortheSubmissionandFormatofThesis.pdf)). However, this may also be of use to Undergraduate and Postgraduate students.

I hope we can build up common knowledge, and share our expertise. If you have a handy tip or trick you would like to share, please raise a Pull Request or email me at [matthew.forshaw@ncl.ac.uk](matthew.forshaw@ncl.ac.uk).

An example of a thesis prepared using thsi template can be found here.

Forshaw, Matthew. Operating Policies for Energy Efficient Large Scale Computing. Diss. Newcastle University, 2015.
http://mattforshaw.com/publications/forshaw2015operating.html

## Starting point
The suggested starting point is the CUED LaTeX template by Krishna Kumar, available at https://github.com/kks32/phd-thesis-template. This template is mature, well-maintained and has been used successfully within our School on a number of occasions.

You can either download the template as a zip file, or you can fork the repository to your own Github account (recommended).

### 1.1. Custom margins

To add custom margins, in accordance with the guidelines, add the ````custommargin```` option to your documentclass at the top of ````thesis.tex````.

```` \documentclass[a4paper,12pt,times,numbered,print,index,custommargin]{Classes/PhDThesisPSnPDF} ````


Finally, in your ```` Preamble/Preamble.tex````, set the custom margin as follows:

```` 
% Add `custommargin' in the document class options to use this section
% Set {innerside margin / outerside margin / topmargin / bottom margin}  and
% other page dimensions
\ifsetCustomMargin
  \RequirePackage[left=30mm,right=20mm,top=20mm,bottom=20mm]{geometry}
  \setFancyHdr % To apply fancy header after geometry package is loaded
\fi
````
