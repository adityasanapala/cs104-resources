# Lab 11 - LaTeX, Spreadsheets

## LaTeX

For this activity, you are required to replicate the given pdf "assignment.pdf".

You have to fill up the "main.tex" and "references. bib" file, which can generate a paf as close as possible to "assignment.pdf".

Below is the detailed description of the document you need to create. Read all the instructions before you begin with the activity.

All the packages required for this activity are already imported in the given "main.tex" file. You shouldn't and mustn't import any other packages.

Following are the major components in each part of the document, which would be considered for evaluation:

1) Preamble

-> Title

-> Author's name

-> Table of contents

2) Section 1 : Introduction

-> List of topics

3) Section 2 : Transformation of Random Variable

-> Three mathematical equations (extra weightage for the last one)

-> 1 Footnote

-> 1 Citation

4) Section 3 : Multi-variate Gaussian Distribution

-> 3 subsections

-> 2 Citations

-> Subfigures

-> Table

-> Equation 2 (last equation)

5) Headers and Footers for each page (except first one)

-> Left header: "Transformation of R.V. and Multivariate Gaussian"

-> Right header : "<Your name>"

-> Footer: Page number

6) References for all the citations (there are 3 citations)

Other details amd resources:

- For cases in equation refer: https://www.overleaf.com/latex/examples/cases/nndqpbymnchn

- For footnote: https://www.overleaf.com/learn/latex/Footnotes#The_\footnote_command

-> Subfigures (two figures in a row) :

https://www.overleaf.com/learn/latex/How_to_Write_a_Thesis_in_LaTeX_(Part_3)%3A_Figures%2C_Subfigures_and_Tables#Subfigures

- Images are provided in the "images" folder

- Need not worry about exact size of the images

-> Bibliography management and citations: https://www.overleaf.com/learn/latex/Bibliography_management_with_bibtex

-> Customizing header and footer: https://tex.stackexchange.com/questions/87768/creating-running-headers-and-footers-but-not-on-the-first-page#:~:t%D0%B5%D1%85t=%255Cuse%D1%80a%D1%81k%D0%B0g%D0%B5%257Bfan%D1%81yhdr%257D%250%D0%90%255Cpag%D0%B5styl%D0%B5%257Bfancy%257D%250%D0%90%255CIhead%257BThis%2520is%2520my%2520name%257D%250A%255Crheac


-> Cross-referencing (references to tables, figures or other sections): https://en.wikibooks.org/wiki/LaTeX/Labels_and_Cross-referencing

-> For citations and references at the end, add 3 references(any) in "references.bib" file. Cite them at the places given in "assignment.pdf"

For equations without numbers (like the first 3 equations of section 1), use display math mode: V... \

For equation with numbers (like the last equation on section 1), use the "equation" environment : Ibegin{equation}... lend{equation}

For any component of the document, refer to the resources given above BEFORE finding other solutions available online.

Usage :

pdflatex main

bibtex main

pdflatex main

pdflatex main

Grading details: Your submission will graded on the basis of the certain tags in the "main.tex" file and "references. bib", though

it must generate a pof without any errors, warnings are acceptable.

Hence, in most cases exact match between your rendered pdf and "assignment.pdf" is not considered, yet it is advisable to create your pdf as similar as possible to the given "assignment.pdf".



## Spreadsheets

Important Note:-

To solve this lab, Kindly use the office application installed on your machine, if available.

Open the folder (can be done by clicking "Open Directory" option from CLab window), and open Employee.xlsx file and then complete the required actions mentioned in problem statement and save it.

In case if there is no preinstalled office application, use online tools like google sheets.

Navigate to the site "https://docs.google.com/spreadsheets/", and select new blank spreadsheet.

Navigate to File > Open > Upload and browse Employee.xlsx in the folder.

Complete the required tasks and download a copy to local (File > Download > Microsoft Excel(.xIsx)). This would be present in the downloads folder.

Copy it and replace the original file. Make sure the file name is Employee.xIsx.

Problem Statement

In the excel named "Employee.xisx",

Column A contains Employee ID, followed by their first name, Last Name, Salary and ID of their manager. Note that the ID of the manager refers to the employee id of a person in the same sheet.

In Column F, you need to fill their Manager full name (First Name & Last Name separated by space)

For example,

The first name of Manager is Kameswari and the last name is Chebrolu. The full name in column F needs to be "Kameswari Chebrolu" (Excluding quotes)

For the CEO of the company, the manager ID will be 0. For a CEO you need to fill in his own name as manager name.

Proper error handling :-

→> If manager ID is not found, The respective cell needs to be filled by "Not Found" (Excluding quotes).

Post this sort the rows based on employee's Salary in decreasing order, then by their First name in alphabetical order to resolve the tie. You can assume the tie if any breaks by First Name.































