---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "LaTeX"
subtitle: "A high-quality typesetting system"
summary: "Post about LaTeX"
authors: [Garut A. I.]
tags: []
categories: []
date: 2022-05-14T14:22:56+03:00
lastmod: 2022-05-14T14:22:56+03:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---

![LaTeX_logo](LaTeX_project_logo_bird.svg.png)

## Overview

LaTeX is a software system for document preparation. When writing, the writer uses plain text as opposed to the formatted text found in "What You See Is What You Get" word processors like Microsoft Word, LibreOffice Writer and Apple Pages. The writer uses markup tagging conventions to define the general structure of a document to stylise text throughout a document (such as bold and italics), and to add citations and cross-references. A TeX distribution such as TeX Live or MiKTeX is used to produce an output file (such as PDF or DVI) suitable for printing or digital distribution.

LaTeX is widely used in academia for the communication and publication of scientific documents in many fields, including mathematics, computer science, engineering, physics, chemistry, economics, linguistics, quantitative psychology, philosophy, and political science. It also has a prominent role in the preparation and publication of books and articles that contain complex multilingual materials, such as Sanskrit and Greek. LaTeX uses the TeX typesetting program for formatting its output, and is itself written in the TeX macro language.

LaTeX can be used as a standalone document preparation system, or as an intermediate format. In the latter role, for example, it is sometimes used as part of a pipeline for translating DocBook and other XML-based formats to PDF. The typesetting system offers programmable desktop publishing features and extensive facilities for automating most aspects of typesetting and desktop publishing, including numbering and cross-referencing of tables and figures, chapter and section headings, the inclusion of graphics, page layout, indexing and bibliographies.

Like TeX, LaTeX started as a writing tool for mathematicians and computer scientists, but even from early in its development, it has also been taken up by scholars who needed to write documents that include complex math expressions or non-Latin scripts, such as Arabic, Devanagari and Chinese.

LaTeX is intended to provide a high-level, descriptive markup language that accesses the power of TeX in an easier way for writers. In essence, TeX handles the layout side, while LaTeX handles the content side for document processing. LaTeX comprises a collection of TeX macros and a program to process LaTeX documents, and because the plain TeX formatting commands are elementary, it provides authors with ready-made commands for formatting and layout requirements such as chapter headings, footnotes, cross-references and bibliographies.

## Typesetting system

LaTeX attempts to follow the design philosophy of separating presentation from content, so that authors can focus on the content of what they are writing without attending simultaneously to its visual appearance. In preparing a LaTeX document, the author specifies the logical structure using simple, familiar concepts such as chapter, section, table, figure, etc., and lets the LaTeX system handle the formatting and layout of these structures. As a result, it encourages the separation of the layout from the content - while still allowing manual typesetting adjustments whenever needed. This concept is similar to the mechanism by which many word processors allow styles to be defined globally for an entire document, or the use of Cascading Style Sheets in styling HTML documents.

The LaTeX system is a markup language that handles typesetting and rendering, and can be arbitrarily extended by using the underlying macro language to develop custom macros such as new environments and commands. Such macros are often collected into packages, which could then be made available to address some specific typesetting needs such as the formatting of complex mathematical expressions or graphics (e.g., the use of the align environment provided by the amsmath package to produce aligned equations).

In order to create a document in LaTeX, you first write a file, say document.tex, using your preferred text editor. Then you give your document.tex file as input to the TeX program (with the LaTeX macros loaded), which prompts TeX to write out a file suitable for onscreen viewing or printing. This write-format-preview cycle is one of the chief ways in which working with LaTeX differs from the What-You-See-Is-What-You-Get (WYSIWYG) style of document editing. It is similar to the code-compile-execute cycle known to computer programmers. Today, many LaTeX-aware editing programs make this cycle a simple matter through the pressing of a single key, while showing the output preview on the screen beside the input window. Some online LaTeX editors even automatically refresh the preview, while other online tools provide incremental editing in-place, mixed in with the preview in a streamlined single window.

## Related software

As a macro package, LaTeX provides a set of macros for TeX to interpret. There are many other macro packages for TeX, including Plain TeX, GNU Texinfo, AMSTeX, and ConTeXt.

When TeX "compiles" a document, it follows (from the user's point of view) the following processing sequence: Macros → TeX → Driver → Output. Different implementations of each of these steps are typically available in TeX distributions. Traditional TeX will output a DVI file, which is usually converted to a PostScript file. More recently, Hàn Thế Thành and others have written a new implementation of TeX called pdfTeX, which also outputs to PDF and takes advantage of features available in that format. The XeTeX engine developed by Jonathan Kew, on the other hand, merges modern font technologies and Unicode with TeX.

The default font for LaTeX is Knuth's Computer Modern, which gives default documents created with LaTeX the same distinctive look as those created with plain TeX. XeTeX allows the use of OpenType and TrueType (that is, outlined) fonts for output files.

There are also many editors for LaTeX, some of which are offline, source-code-based while others are online, partial-WYSIWYG-based. For more, see Comparison of TeX editors.

## Compatibility and converters

LaTeX documents (*.tex) can be opened with any text editor. They consist of plain text and do not contain hidden formatting codes or binary instructions. Additionally, TeX documents can be shared by rendering the LaTeX file to Rich Text Format (*.rtf), XML, or the .cls container format. This can be done using the free software programs LaTeX2RTF or TeX4ht. LaTeX can also be rendered to PDF files using the LaTeX extension pdfLaTeX. LaTeX files containing Unicode text can be processed into PDFs with the inputenc package, or by the TeX extensions XeLaTeX and LuaLaTeX.

HeVeA is a converter written in Ocaml that converts LaTeX documents to HTML5. It is licensed under the Q Public License.
LaTeX2HTML is a converter written in Perl that converts LaTeX documents to HTML. This way, e.g., scientific papers—primarily typeset for printing—can be placed on the Web for online viewing. It is licensed under GNU GPL v2. The latest updates are available from CTAN.
LaTeXML is a free, public domain software, written in Perl, which converts LaTeX documents to a variety of structured formats, including HTML5 (with MathML), epub (encapsulation of HTML), jats, tei.
Pandoc is a 'universal document converter' able to transform LaTeX into many different file formats, including HTML5, epub, rtf and docx. It is licensed under GNU GPL v2.
LaTeX has become the de facto standard to typeset mathematical expression in scientific documents. Hence, there are several conversion tools focusing on mathematical LaTeX expressions, such as converters to MathML or Computer Algebra System.

MathJax is a JavaScript library for converting LaTeX to MathML, picture formats, or HTML.
The Wikimedia foundation uses it to build Mathoid, a web-service converter using Node.js that converts math inputs, such as LaTeX, to MathML and picture formats, including SVG and PNG. Mathoid is used in Wikipedia to render math.
KaTeX is a JavaScript library for converting LaTeX to HTML and MathML. It is developed by the Khan Academy, and is among the fastest LaTeX to HTML converters.