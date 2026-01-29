# LaTeX worksheet template
A LaTeX template for worksheets and class tests to be used in schools

## Installation
There are multiple options to install the template.
The easiest method is to simply put the file `worksheet.sty` in the directory you wish to create your document in.
Please refer to [this guide](https://en.wikibooks.org/wiki/LaTeX/Installing_Extra_Packages) for a global installation.

## Usage
To create a document using the template, include the package in the head of your LaTeX file using `\usepackage{worksheet}`.
The package provides several new commands:
- `\makeheader{subject}{topic}` creates the document header with the given subject and topic.
- **Tasks**: There are 5 different commands to denote a task.
  - `\singletask{title}` creates a task to be done alone.
  - `\partnertask{title}` creates a task to be done in partner work.
  - `\grouptask{title}` creates a task to be done in a group.
  - `\bonustask{title}` creates a bonus task.
  - `\testtask{title}{points}` creates a class test task with a specific amount of points.
- **Boxes**: There are two types of boxes used to show information:
  - ```\begin{warning}{title}
  content
\end{warning}``` denotes a warning
  - ```\begin{hint}{title}
  content
\end{content}``` denotes a hint used to give additional information to the students
- **Fields**: You can also create spaces for students to write or draw on.
  All areas default to a length of 5cm in case no argument is given.
  - `\checkered[length]` creates a checkered area with the given length.
  - `\lines[length]` creates lines to write on, spaced 1cm apart.
  - `\boxarea[length]` creates an empty box without any guidelines.
