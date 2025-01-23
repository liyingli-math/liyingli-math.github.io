+++
title = "Scientific workflow in Emacs"
draft = false
showtoc = true
+++

> Vim is the editor God, and Emacs is God's editor.

I "live" in [Emacs](https://www.gnu.org/software/emacs/) everyday. I use it to

-   write LaTeX,
-   take notes,
-   read and annotate PDFs,
-   perform personal knowledge management ([Zettlekasten system](https://en.wikipedia.org/wiki/Zettelkasten)),
-   write codes (Python, Julia, ...),
-   build static sites (like this one),
-   read and send emails,
-   do GTD and time management,

and more.
For those who are looking for a more productive research workflow,
I hope that this article can be inspiring and introduce you to the Emacs's world of infinite possibilities.


## Life in Emacs {#life-in-emacs}


### LaTeX {#latex}

I started using Emacs as a LaTeX editor. One day I found myself capable of typing LaTeX fast enough to keep up with math lectures, and sine then, Emacs has been an indispensable part of my research workflow.


#### Overview {#overview}

The three packages AUCTeX, CDLaTeX and PDF-tools give Emacs the core functionality to write LaTeX.

![LaTeX](./LaTeX.gif)

-   The left part shows the LaTeX file and the right the compiled PDF (PDF-tools).
-   At startup, section contents are hidden to make it easier to navigate; you can unfold any section to start editing.
-   <kbd>C-c C-v</kbd> to jump from source to PDF (note the little red arrow and the highlighted text); double-click to jump from PDF to source.
-   Prettify: show Unicode symbols like `ℱ`, `∞` to replace math macros like `\mathcal{F}`, `\infty`.
-   Fold LaTeX macros, so `\label{eq:XXX}`, `\cref{eq:XXX}` becomes `[l]`, `[cr]`.

I insert almost all macros using Emacs commands, so the invisible parts can stay error-free. See below.


#### Insert Macros effortlessly {#insert-macros-effortlessly}

Use CDLaTeX to insert macros fast and accurately.

![CDLaTeX](./CDLaTeX.gif)

-   <kbd>\`+&lt;key&gt;</kbd> inserts Greek letters and symbols.
-   <kbd>&lt;keyword&gt;+TAB</kbd> expands to a macro or an environment template. Example:
    -   <kbd>equ*+TAB</kbd> inserts the `equation*` environment.
    -   <kbd>fr+TAB</kbd> expands to `\frac{}{}`.
-   <kbd>&lt;key&gt;+'</kbd> or <kbd>'+&lt;key&gt;</kbd> inserts modified letters. Example: <kbd>R'c</kbd> inserts `\mathcal{R}`.

All these shortcuts are highly customizable.


#### Cross Reference {#cross-reference}


## Learning and configuration {#learning-and-configuration}
