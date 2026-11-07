# Wasur

The LaTeX style I use for my notes. It sets everything in iA Writer Quattro and iA Writer Mono, keeps the spacing tight and adds the shortcuts I use for physics notes.

## Use

It needs XeLaTeX or LuaLaTeX. pdfLaTeX is not supported.

Install the fonts in `fonts/` or put them in your local `texmf/fonts/truetype/`, and put `wasur.sty` next to your document or in `texmf/tex/latex/wasur/`.

```latex
\documentclass[a4paper, 12pt]{article}
\usepackage{wasur}

\begin{document}

\quicknote[7 November 2026]{Spinors}
A dated note with a \term{defined term} and $\ket{\psi} = \pauliX \ket{0}$.

\end{document}
```

## Options

- `relaxed` adds some space around headings, lists and display math. By default it is all tight.
- `static` uses the static fonts instead of the variable ones. They are not in this repo, but you can get them from [iA-Fonts](https://github.com/iaolo/iA-Fonts).

## Commands

| | |
| --- | --- |
| Notes | `\quicknote[date]{title}`, `\term{}`, `\todo{}` |
| Number sets | `\R`, `\C`, `\N`, `\Z`, `\Q` |
| Groups and algebras | `\SU{n}`, `\SO{n}`, `\su{n}`, `\so{n}`, `\SUr{n}`, `\SOr{n}`, `\GL{n}` |
| Dirac notation | `\ket{}`, `\bra{}`, `\braket{}{}`, `\ketbra{}{}` |
| Operators | `\tr`, `\diag`, `\sgn`, `\Id`, `\herm{}`, `\transp{}`, `\conj{}`, `\comm{}{}`, `\acomm{}{}` |
| Delimiters | `\abs{}`, `\norm{}`, `\inner{}` |
| Derivatives | `\dd`, `\dv{}{}`, `\pdv{}{}` |
| Pauli matrices | `\pauliX`, `\pauliY`, `\pauliZ` |

## Fonts

The fonts are iA Writer, by Information Architects Inc., based on IBM Plex. They are unmodified and licensed under the SIL Open Font License, see [`fonts/LICENSE.md`](fonts/LICENSE.md).
