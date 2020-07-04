# random-exam
Use LaTeX and conditional statements to generate customized exams

Use `pdflatex` with a string input that defines two variables:
* `seed`: Generation Seed.  Meant for randomization.
* `user`: Constant for the user.  Meant for Student identifiers (e.g., Matric).
* `mode`: Generation Mode.  Meant for conditional document generation.  i.e., decide whether to create the `exam` or the `solution`.

By default, generates with `seed` = 1, `student` = "A01234567X" and `mode` = "Exam".

## Generate output

`pdflatex "\def\seed{1}\def\mode{Exam}\def\user{A01234567X} \input{exam.tex}"`
`pdflatex "\def\seed{2}\def\mode{Answer}\def\user{A9876544Y} \input{exam.tex}"`
