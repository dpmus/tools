# Digital Tools for Humanities Research

## Citation and Source Material Management

- [Zotero](https://zotero.org) -- Open-Source citation management software
  - Runs on Windows, MacOS, Linux
  - Can manage your PDFs as attachments (see below)
  - Has plugins and integrations for Microsoft Office and LibreOffice
  - Can import citation information automagically from ISBN or DOI
  - [Zotero @ FSU](https://guides.lib.fsu.edu/zotero)
- [Zotmoov](https://github.com/wileyyugioh/zotmoov)
  - Normally, Zotero will store your PDFs in a network of hidden folders and synchronize them to its own, paid cloud storage :(
  - Zotmoov is a Zotero plugin that allows you to choose a different folder on your computer, possibly one connected to OneDrive or Google Drive

## Notes

- [Obsidian](https://obsidian.md)
  - Runs on Windows, MacOS, Linux, and mobile
  - Notes formatted in Markdown (see below)
  - Not open source but freely available with many plugins
  - Allows note linking, 3D visualization, flow charts, sketch boards
  - Stores notes as a folder of text files. If you stop using Obsidian, you can still access them in any other text editor.
  - Wants to sell you its own, paid cloud storage :(

## Word Processors

- [Microsoft Word](https://www.microsoft.com/en-us/microsoft-365/word)
  - Free for University affiliates, subscriptions for everyone else
  - DOCX file format is industry standard for journals and publishers
  - Not open source
  - Pushes cloud storage and now AI
- [LibreOffice](https://www.libreoffice.org/)
  - Open source, free for everyone
  - Uses ODT format by default but highly compatible with DOCX
	- LibreOffice is better at rendering DOCX files than Word is at ODT
  - Excellent PDF export options
  - User interface feels like Word 2003 (a benefit to some...)
- [Scrivener](https://www.literatureandlatte.com/)
  - More like a combination of Obsidian and Word/LibreOffice
  - Allows you to write in snippets, rearrange them, and compile into DOCX and other formats
  - Geared toward novel and book writers but can be used to organize research
  - Not open source
  - One-time fee, must buy versions for MacOS, Windows, and mobile separately
  - Academic discount

## Plaintext Workflow

The following tools are for a different way of working. They involve drafting in a text editor and then exporting to DOCX, PDF, HTML. Originally developed by bloggers and digital-first authors but gaining traction among academics. Parallel to the LATEX and [Overleaf](https://www.overleaf.com/) workflow used in the sciences.

### Markdown

- Markdown is a way of formatting plain text that allows for basic formatting, like **bold**, *italics*, headings, and footnotes^[Sample footnote].
- You use a plain text editor to write in Markdown. Then, you use a utility---either one built into the text editor itself or a separate program---to convert the markdown to an output format.

### Text Editors

- [Microsoft VSCode](https://code.visualstudio.com/) -- Industry-leading text and code editor
  - Partly open source
  - Windows, MacOS, Linux
  - Tons of plugins and AI Copilot
  - Can customize the appearance for different "languages" (i.e., markdown)
- [Emacs](https://www.gnu.org/software/emacs/)
  - One of the original text editors from the 1980s
  - Fully open source
  - Windows, MacOS, Linux
  - Extremely customizable
	- Can save your settings as a [text file](/extras/.emacs) to transport them to other computers
  - Can be used as an outliner, planner, project manager, email client, etc. etc.
  - Steep learning curve, huge time suck

### Markdown Converter

- [Pandoc](https://pandoc.org/)
  - Open source
  - Command-line utility for converting between dozens of different file formats. Ex., markdown to [DOCX](/samples/README.docx), [ODT](/samples/README.odt), [RTF](/samples/README.rtf), [HTML](/samples/README.html), [PDF](/samples/README.pdf) (via LaTex).
	- `pandoc sample.md -o sample.docx`
  - Can use a [template](/extras/manuscript-template.docx) to standardize output formatting
	- `pandoc sample.md -o sample.docx --reference-doc=manuscript-template.docx`
	
### Considerations

#### Advantages

- Distraction-free writing
- Draft first, format later
- Markdown text files are small
- Citation management
  - You can curate your bibliography in a BibTex file, embed citation keys into your Markdown manuscript, and then compile the citations automatically as part of the export process
- Sync, version control, collaboration with `git` and [GitHub](https://github.com)
- Easy export to a variety of formats: DOCX for publishers, PDF for printing, HTML for web
- Outputs accessible DOCX files with Styles used correctly
- Markdown is spreading (Zotero, Obsidian, web developing)
- Learn digital humanities tools
- Open source tools are free to use and privacy-friendly

#### Disadvantages

- **Warning:** Learning curve (time suck)
- Customization (time suck)
- Need to convert to DOCX for collaboration and feedback (time suck)
