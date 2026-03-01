# Awesome LaTeX Tools [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A handpicked collection of outstanding tools, editors, packages, and resources for the [LaTeX typesetting ecosystem](https://www.latex-project.org/) and scientific writing workflows.

Whether you're drafting a dissertation, preparing a conference paper, or typesetting a book, this list has you covered with battle-tested software and hidden gems alike.

## Contents

- [Getting Started](#getting-started)
- [TeX Distributions](#tex-distributions)
- [Containerized Environments](#containerized-environments)
- [Typesetting Engines](#typesetting-engines)
  - [Modern Alternatives](#modern-alternatives)
  - [Math on the Web](#math-on-the-web)
- [Writing Environments](#writing-environments)
  - [Dedicated LaTeX Editors](#dedicated-latex-editors)
  - [Multipurpose Code Editors](#multipurpose-code-editors)
  - [Browser-Based Editors](#browser-based-editors)
- [Citation & Bibliography Management](#citation--bibliography-management)
- [Compilation & Build Automation](#compilation--build-automation)
  - [CI/CD for LaTeX](#cicd-for-latex)
- [Utilities & Helpers](#utilities--helpers)
  - [Linting & Quality Checks](#linting--quality-checks)
  - [Equation-Focused Tools](#equation-focused-tools)
- [Visual & GUI Tools for LaTeX](#visual--gui-tools-for-latex)
- [Package Ecosystem](#package-ecosystem)
  - [Cross-References](#cross-references)
  - [Tables & Tabular Data](#tables--tabular-data)
  - [Figures & Diagrams](#figures--diagrams)
    - [PSTricks](#pstricks)
    - [TikZ & PGF](#tikz--pgf)
  - [Code Listings](#code-listings)
  - [Typographic Refinement](#typographic-refinement)
  - [Slide Decks & Presentations](#slide-decks--presentations)
- [Starter Templates](#starter-templates)
- [Symbol Lookup](#symbol-lookup)
- [Community & Reference Material](#community--reference-material)
- [Eye Candy & Showcases](#eye-candy--showcases)
- [Learning Paths](#learning-paths)
- [Essential Reading](#essential-reading)
- [Blogs & Newsletters](#blogs--newsletters)
- [Community Hubs](#community-hubs)

## Getting Started

New to LaTeX? Jump to the [Learning Paths](#learning-paths) section for beginner-friendly guides.

## TeX Distributions

Your first step is installing a TeX distribution — it bundles the compiler, fonts, and thousands of packages.

- [MacTeX](https://tug.org/mactex/) — The go-to distribution for macOS users. Ships TeXLive core plus Mac-native utilities.
- [TeX Live](https://www.tug.org/texlive/) — The standard distribution across Linux and Unix systems. Also runs on Windows.
- [MikTeX](https://miktex.org) — A popular choice on Windows with on-the-fly package installation. Cross-platform builds exist for Mac and Linux too.

## Containerized Environments

Skip local installation entirely — spin up a ready-to-go LaTeX setup with Docker.

- [reitzig/texlive-docker](https://github.com/reitzig/texlive-docker) — Lightweight TeXLive image with on-demand package installation.
- [Island of TeX/texlive](https://gitlab.com/islandoftex/images/texlive) — Full TeXLive system on a Debian base.
- [dante-ev/docker-texlive](https://github.com/dante-ev/docker-texlive) — Complete TeXLive plus pandoc, perl, and python pre-bundled on Debian.

## Typesetting Engines

The engine decides how your `.tex` source becomes a finished document.

- [pdfTeX](https://www.tug.org/applications/pdftex/) — The workhorse engine that outputs PDF directly. Default choice for most users today.
- [XeTeX](http://xetex.sourceforge.net) — Unlocks system fonts and full Unicode support — ideal for multilingual documents.
- [LuaTeX](https://www.luatex.org) — Embeds a Lua scripting layer alongside modern Unicode and font handling.
- [tectonic](https://tectonic-typesetting.github.io/en-US/) — A modern, self-contained engine built in Rust on XeTeX and TeXLive. Auto-downloads packages on demand.

### Modern Alternatives

Tools that reimagine scientific typesetting beyond the traditional TeX workflow.

- [Typst](https://typst.app) ([GitHub](https://github.com/typst/typst)) — A markup-based typesetting system designed as a modern replacement for LaTeX. Compiles in milliseconds, produces clean PDFs, and has a growing package ecosystem. Most journals still require `.tex` submissions, but Typst is an excellent choice for theses, internal reports, and preprints.

### Math on the Web

Render LaTeX-quality equations outside of PDF.

- [MathJax](https://www.mathjax.org) — The gold-standard JavaScript library for rendering math in browsers. Crisp output everywhere.
- [KaTeX](https://khan.github.io/KaTeX/) — Khan Academy's lightning-fast math renderer. Outputs pure HTML — no images.
- [Auto-LaTeX Equations with Google Docs](https://sites.google.com/site/autolatexequations) — Drop high-fidelity math equations straight into Google Docs.
- [Franklin.jl](https://franklinjl.org/) — Julia-powered static site generator with native KaTeX, code evaluation, and LaTeX-like commands.
- [xhub](https://github.com/nschloe/xhub) — Browser extension that activates LaTeX rendering on GitHub pages.

## Writing Environments

Life's too short to typeset in Notepad. Here are the best places to write LaTeX.

### Dedicated LaTeX Editors

Purpose-built for `.tex` files.

- [TeXStudio](https://www.texstudio.org) — The most actively developed open-source LaTeX IDE. Rich autocompletion, integrated viewer, and custom build commands.
- [TeXMaker](https://www.xm1math.net/texmaker/) — Solid cross-platform editor with an integrated PDF viewer and real-time preview.
- [Kile](https://kile.sourceforge.io) — Feature-rich editor born on KDE/Linux that also runs well on Windows and macOS.
- [LyX](https://www.lyx.org) — A WYSIWYM front-end: you write structured content, LaTeX handles the typesetting behind the scenes.
- [Texifier](https://www.texifier.com/) — Polished commercial editor for Apple platforms with document outlines, synced PDF, and device sync (macOS).
- [WinEdt](https://www.winedt.com) — A beloved editor with a devoted following (Windows).
- [TeXShop](https://pages.uoregon.edu/koch/texshop/) — Clean, no-frills editor bundled with MacTeX (macOS).
- [TeXWorks](https://www.tug.org/texworks/) — Minimalist cross-platform editor inspired by TeXShop.

### Multipurpose Code Editors

General-purpose editors that handle LaTeX alongside everything else.

- [VS Code](https://code.visualstudio.com/)
  - [LaTeX Workshop](https://github.com/James-Yu/LaTeX-Workshop) — Rich LaTeX extension with build automation, preview, and IntelliSense.
  - [LTeX](https://marketplace.visualstudio.com/items?itemName=valentjn.vscode-ltex) — Grammar and spell checking powered by LanguageTool.
  - [a-nau/latex-devcontainer](https://github.com/a-nau/latex-devcontainer) — Dev Container config for zero-install LaTeX editing.

- [Zed](https://zed.dev)
  - [LaTeX extension](https://zed.dev/extensions/latex) — Syntax highlighting and language server support. Auto-compile on save with live preview.
  - [TeXpresso](https://zed.dev/extensions/texpresso) — Live preview of LaTeX documents inside the editor.

- [Vim](https://www.vim.org) / [Neovim](https://neovim.io)
  - [vimtex](https://github.com/lervag/vimtex) — The definitive Vim/Neovim LaTeX plugin. Compilation, live preview, forward/inverse search, and much more.

- [Emacs](https://www.gnu.org/software/emacs/)
  - [AUCTeX](https://www.gnu.org/software/auctex/) — The definitive Emacs LaTeX mode — includes equation and figure previews.
  - [RefTeX](https://www.gnu.org/software/auctex/reftex) — Companion to AUCTeX for managing labels, references, and citations.

- [Sublime Text](https://www.sublimetext.com)
  - [LaTeXTools](https://github.com/SublimeText/LaTeXTools) — Well-maintained free LaTeX plugin with build and preview support.

- [IntelliJ](https://www.jetbrains.com/idea/)
  - [TeXiFy-IDEA](https://github.com/Hannah-Sten/TeXiFy-IDEA) — Full-featured free LaTeX support inside any JetBrains IDE.

- [texlab](https://github.com/latex-lsp/texlab) — Language Server Protocol implementation for LaTeX. Works with any LSP-capable editor.

### Browser-Based Editors

Write and compile from any device with a browser.

- [Overleaf](https://www.overleaf.com) — The most widely used online LaTeX platform. Supports visual editing, real-time collaboration, and git sync.
  - [olcli](https://github.com/aloth/olcli) — CLI companion for Overleaf: sync, manage, and compile from your terminal.
  - [Underleaf](https://www.underleaf.ai/) — AI-powered Chrome extension for Overleaf that adds smart writing assistance, equation OCR, and dark mode.
- [Prism](https://prism.openai.com/) — Free AI-native LaTeX workspace by OpenAI. Project-aware AI assistance, image-to-LaTeX conversion, and unlimited collaborators.
- [CoCalc](https://cocalc.com/features/latex-editor) — Online LaTeX editor with real-time collaboration, embedded computation (Python, Sage, R), and full version history.
- [Octree](https://useoctree.com) — AI-assisted online LaTeX editor with intelligent autocomplete and error detection.
- [Authorea](https://www.authorea.com) — Collaborative writing platform with integrated version control and references.
- [SpicyChai LaTeX](https://latex.spicychai.com) — Online LaTeX editor with AI writing assistance, real-time PDF preview, and templates for papers, theses, and presentations.
- [Papeeria](https://papeeria.com) — Online editor with built-in version control.
- [WebLaTeX](https://github.com/sanjib-sen/weblatex) — VS Code in the browser via GitHub Codespaces with Git, Copilot, and live collaboration.
- [JaxEdit](https://zohooo.github.io/jaxedit/) — Lightweight browser editor with live preview and presentation mode.

## Citation & Bibliography Management

Taming your references so you don't have to.

- [Zotero](https://www.zotero.org) — Captures references from your browser, syncs across devices, and exports to BibTeX. The most popular free option.
- [JabRef](https://www.jabref.org) — Powerful open-source BibTeX manager. Runs everywhere Java does.
- [Papis](https://github.com/papis/papis) — Highly scriptable, command-line-first library manager in Python. Multiple GUIs available.
- [BibDesk](http://bibdesk.sourceforge.net) — Native macOS bibliography editor that integrates tightly with the system.
- [Mendeley](https://www.mendeley.com) — Reference manager and PDF organizer with cloud sync and BibTeX export.
- [betterbib](https://github.com/nschloe/betterbib) — CLI tool that cleans up and enriches your `.bib` files using online databases.
- [OneCite](https://github.com/HzaCode/OneCite) — All-in-one citation toolkit: feed it a DOI, arXiv ID, or title and get BibTeX, APA, or MLA output.

## Compilation & Build Automation

Automate the tedious compile-recompile-compile cycle.

- [latexmk](https://www.ctan.org/pkg/latexmk) — The de facto standard build tool, used under the hood by most editors.
- [Arara](https://www.ctan.org/pkg/arara) ([GitHub](https://github.com/islandoftex/arara)) — Declare build steps inside your document. Easy to extend.
- [tectonic](https://tectonic-typesetting.github.io/en-US/) — Also functions as a build tool: auto-downloads packages, determines the right number of compilation passes, and produces reproducible builds.

### CI/CD for LaTeX

- [xu-cheng/latex-action](https://github.com/xu-cheng/latex-action) — GitHub Action that compiles LaTeX documents in your CI pipeline.
- [dante-ev/latex-action](https://github.com/dante-ev/latex-action) — DANTE's GitHub Action with a full TeXLive environment plus perl and python.

## Utilities & Helpers

- [Pandoc](https://pandoc.org) — The Swiss Army knife of document conversion: LaTeX, Word, Markdown, HTML, and dozens more.
- [CaTeX](https://github.com/Alexis-benoist/CaTeX) — Merges multiple LaTeX files into one, intelligently combining preambles.

### Linting & Quality Checks

- [ChkTeX](https://www.nongnu.org/chktex/) — Static analysis tool that catches common LaTeX pitfalls.
- [blacktex](https://github.com/nschloe/blacktex) — Auto-formatter that scrubs anti-patterns from your `.tex` files.
- [TeXtidote](https://github.com/sylvainhalle/textidote) — Spelling, grammar, and style checker purpose-built for LaTeX.

### Equation-Focused Tools

- [Mathpix](https://mathpix.com) — Industry-leading OCR for math, tables, and scientific notation. Converts images and PDFs to LaTeX, Markdown, or DOCX.
- [pix2tex](https://lukas-blecher.github.io/LaTeX-OCR/) — Open-source OCR that reads math from images and outputs LaTeX code.
- [Image to LaTeX](https://www.underleaf.ai/tools/image-to-latex) — AI-driven converter for handwritten notes, equations, and tables.
- [Codecogs Eqn Editor](https://editor.codecogs.com/) — Point-and-click online equation editor that exports images.
- [LaTeXiT](https://www.chachatelier.fr/latexit/) — Drag rendered equations (PDF, PNG) into any Mac app.
- [LaTeX to Image](https://thomasahle.com/latex2png/) — Online converter: LaTeX to PNG, JPEG, or SVG. Includes a symbol palette.
- [EqualX](https://equalx.sourceforge.io/) — Desktop GUI for composing equations.
- [KLaTeXFormula](https://klatexformula.sourceforge.io) — Cross-platform equation-to-image converter.

## Visual & GUI Tools for LaTeX

Draw diagrams and figures with LaTeX-native output.

- [IPE](https://ipe.otfried.org) — Precision drawing tool designed around LaTeX text integration.
- [GeoGebra](https://www.geogebra.org/) — Interactive geometry app that can export directly to TikZ.
- [TikZiT](https://tikzit.github.io) — Lightweight GUI for creating PGF/TikZ graphs and string diagrams.
- [TikzEdt](https://www.tikzedt.org) ([GitHub](https://github.com/hchapman/tikzedt)) — Side-by-side WYSIWYG and code editor for TikZ.
- [LaTeXDraw](https://latexdraw.sourceforge.net/) — Vector drawing application that treats LaTeX as a first-class output format.
- [Dia](https://wiki.gnome.org/Apps/Dia) — General-purpose diagramming tool with PSTricks and MetaPost export.
- [Vexlio](https://vexlio.com/) — Diagram editor with native LaTeX equation support and easy export.

## Package Ecosystem

- [CTAN](https://www.ctan.org) — The Comprehensive TeX Archive Network: the central hub for every TeX package and its documentation.

### Cross-References

- [hyperref](https://www.ctan.org/pkg/hyperref) — The essential package for clickable cross-references, internal links, and PDF metadata. Load it last in your preamble.
- [cleveref](https://www.ctan.org/pkg/cleveref) — Smarter referencing: `\cref{fig:example}` automatically prepends "Figure", "Table", "Equation", etc. — and handles plural forms too.
- [varioref](https://www.ctan.org/pkg/varioref) — Adds contextual page references: `\vref{sec:intro}` outputs "Section 2 on page 5" or "on the next page" as appropriate.

### Tables & Tabular Data

- [Tables Generator](https://www.tablesgenerator.com) — Visual web app: design your table, copy out the LaTeX (or Markdown, or HTML).
- [Excel2LaTeX](https://www.ctan.org/pkg/excel2latex?lang=en) — Macro that converts Excel spreadsheets into LaTeX `tabular` code.
- [csv2latex](https://www.ctan.org/pkg/csv2latex) — Script that converts clipboard spreadsheet data (Excel, LibreOffice, Numbers) into LaTeX table code. Works with plain tables, booktabs, longtable, and raw cells.
- [pgfplotstable](https://www.ctan.org/pkg/pgfplotstable?lang=en) — Package for rendering data tables with configurable formatting — reads CSV natively.

### Figures & Diagrams

#### PSTricks

A mature library for generating publication-quality figures within PostScript and DVI workflows.

#### TikZ & PGF

The dominant LaTeX graphics package. Rich plugin ecosystem, works seamlessly with `pdflatex`.

- [pgfplots](http://pgfplots.sourceforge.net) — Feature-rich plotting library in the TikZ style. Reads CSV and computes on the fly.
- [TeXample](https://www.texample.net) — Huge gallery of TikZ examples with source code.
- [A very minimal introduction to TikZ (PDF)](https://cremeronline.com/LaTeX/minimaltikz.pdf) — Concise starter guide by Jacques Crémer.
- [PetarV-/TikZ](https://github.com/PetarV-/TikZ) — Gallery of publication-ready PGF/TikZ figures.
- [matlab2tikz](https://github.com/matlab2tikz/matlab2tikz) — Export MATLAB plots as PGFPlots/TikZ.
- [tikzplotlib](https://github.com/nschloe/tikzplotlib) — Export matplotlib figures as PGFPlots/TikZ.
- [TikZBlog](https://latexdraw.com) — Step-by-step drawing tutorials for TikZ.
- [LaTeX en SI](https://sciences-indus-cpge.papanicola.info/-LaTeX-en-SI-) — Specialized TikZ packages for Bode plots, Nyquist diagrams, circuit schematics, and block diagrams (French).

### Code Listings

- [listings](https://www.ctan.org/pkg/listings) — The workhorse package for typesetting source code. Ships with every TeX distribution, no external dependencies. Configurable keyword colors, frames, and captions.
- [minted](https://www.ctan.org/pkg/minted) — Syntax-highlighted code listings powered by [Pygments](https://pygments.org/), supporting 300+ languages. Requires Python and `--shell-escape`.

### Typographic Refinement

- [microtype](https://ctan.org/pkg/microtype) — Enables margin kerning and font expansion for noticeably better-looking paragraphs.

### Slide Decks & Presentations

- [Beamer](https://www.ctan.org/pkg/beamer) ([GitHub](https://github.com/josephwright/beamer)) — The standard LaTeX framework for presentations. Supports themes, overlays, animations, and speaker notes. Works with pdflatex, XeLaTeX, and LuaLaTeX.
- [nics](https://nics.nilcons.com/) — An opinionated Beamer alternative that prioritizes beautiful defaults and simplicity. Excellent docs and cheatsheet.

## Starter Templates

- [LaTeX Templates](https://www.latextemplates.com) — Ready-made templates for papers, posters, CVs, theses, books, slides, and more.
- [Ultimate Beamer Theme List](https://github.com/martinbjeldbak/ultimate-beamer-theme-list) — Catalogue of Beamer themes with PDF previews.
- [LaTeX Beamer Theme Overview](https://github.com/UweZiegenhagen/LaTeX-Beamer-Theme-Overview/blob/main/OVERVIEW.md) — Visual index of every Beamer theme bundled with TeXLive.
- [TeXtured](https://github.com/jdujava/TeXtured) — Clean, structured thesis template with strong typographic choices.

## Symbol Lookup

- [Detexify](https://detexify.kirelabs.org/classify.html) — Sketch a symbol with your mouse and get the LaTeX command back instantly.
- [Comprehensive LaTeX Symbol List](https://www.ctan.org/tex-archive/info/symbols/comprehensive/) — Exhaustive reference of every symbol available in LaTeX. ([A4 PDF](https://mirrors.ctan.org/info/symbols/comprehensive/symbols-a4.pdf) | [Letter PDF](https://mirrors.ctan.org/info/symbols/comprehensive/symbols-letter.pdf))

## Community & Reference Material

- [TUG](https://www.tug.org) — The TeX Users Group: the global community for TeX enthusiasts.
- [TeXDoc](https://texdoc.net) — Search and browse package documentation online.
- [Dickimaw Books: LaTeX resources](https://www.dickimaw-books.com/latexresources.html) — Well-organized overview of essential LaTeX links.
- [LaTeX Cookbook](https://latex-cookbook.net) — Practical examples and code snippets for common tasks.
- [Visual FAQ](https://ctan.org/pkg/visualfaq) — See a formatting problem, click it, and get the TeX FAQ solution.
- [MartinThoma's LaTeX examples](https://github.com/MartinThoma/LaTeX-examples/) — Repository of sample documents covering many scenarios.
- [LaTeX Community Forum](https://latex.org/forum) — Active discussion board for Q&A and tips.
- [BibTeX Style Examples](http://www.cs.stir.ac.uk/~kjt/software/latex/showbst.html) — Side-by-side output of popular `.bst` bibliography styles.
- [TeX World](https://tex.world/) — Portal supported by TUG, DANTE, and GUTenberg.
- [TeXnique](https://texnique.xyz) — Test your LaTeX skills with this typesetting game.

## Eye Candy & Showcases

- [TUG TeX Showcase](https://www.tug.org/texshowcase/) — Official showcase from the TeX Users Group.
- [Awesome LaTeX Drawing](https://github.com/xinychen/awesome-latex-drawing) — Curated collection of academic illustrations made with LaTeX.

## Learning Paths

- [LearnLaTeX.org](https://www.learnlatex.org/) — Interactive browser-based lessons — no install needed.
- [The (Not So) Short Introduction to LaTeX2e](https://mirrors.ctan.org/info/lshort/english/lshort.pdf) — The classic deep-dive introduction (PDF).
- [Begin LaTeX in minutes](https://github.com/luong-komorebi/Begin-Latex-in-minutes) — Quick-start guide for absolute beginners.
- [Getting to Grips with LaTeX](https://www.andy-roberts.net/writing/latex) — Thorough walkthrough of most LaTeX features you'll need.
- [Typst for LaTeX users](https://typst.app/docs/guides/for-latex-users/) — Official migration guide if you're considering Typst.

## Essential Reading

- [Wikibooks: LaTeX](https://en.wikibooks.org/wiki/LaTeX) — Free, community-written reference that rivals any printed book.
- [The LaTeX Companion, F. Mittelbach (2004)](https://www.informit.com/store/latex-companion-9780201362992)
- [LaTeX Graphics Companion, M. Goossens (2007)](https://www.informit.com/store/latex-graphics-companion-9780321508928)
- [TeX by Topic (2007)](https://ctan.org/pkg/texbytopic)
- [TeX for the Impatient (2020)](https://ctan.org/pkg/impatient)
- [Formatting Information (2020)](https://latex.silmaril.ie/formattinginformation) — Continuously updated HTML5 guide to typesetting with LaTeX.

## Blogs & Newsletters

- [TeXblog](https://texblog.net) — Long-running blog covering LaTeX tips and techniques.
- [texblog.org](https://texblog.org) — Tutorials, package spotlights, and code snippets.
- [TeX Talk](https://tex-talk.net) — News and interviews from the TeX Stack Exchange community.
- [TeX Hour](https://texhour.github.io/) — Weekly video meetup for the TeX community.

## Community Hubs

- [TopAnswers TeX](https://topanswers.xyz/tex) — Open-source Q&A platform for TeX questions.
- [LinkedIn: TeX/LaTeX User Group](https://www.linkedin.com/groups/1600297)

---

All trademarks belong to their respective owners.
