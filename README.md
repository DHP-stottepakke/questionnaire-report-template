# Questionnaire Report

This a fork of generic default template for [Data Stewardship Wizard (DSW)](https://ds-wizard.org/) directly transforms answers from a questionnaire into a document while maintaining the structure. It is not tied to any knowledge model. This is a version for an reduced output for leaner documents.

This lean version is following the main release cycle. It is based on the upstream template [ds-wizard/questionnaire-report-template](https://github.com/ds-wizard/questionnaire-report-template) and leaves out question texts, per-question tags, chapter summaries, unselected choices, the separate cover page (HTML/PDF) and the table of contents (LaTeX); list questions with fewer than six sub-questions are rendered as tables.

Version 3.x requires Data Stewardship Wizard 5.0 or newer (template metamodel 19.0); use 2.17.x with DSW 4.x.


## Translations

All texts of the template are marked for translation (source language: English), including month
names in dates (and the `babel` language of the LaTeX format). The Wizard generates the POT file
when the template is released; upload translated PO files as document template locales to get
documents in other languages. Content of the knowledge model and the answers are not translated.


### Original Contributors

* **Marek Suchánek** <[marek.suchanek@ds-wizard.org](mailto:marek.suchanek@ds-wizard.org)>
  * ORCID: [0000-0001-7525-9218](https://orcid.org/0000-0001-7525-9218)
  * GitHub: [@MarekSuchanek](https://github.com/MarekSuchanek)
* **Kryštof Komanec** <[krystof.komanec@ds-wizard.org](mailto:krystof.komanec@ds-wizard.org)>
  * ORCID: [0000-0003-3856-1682](https://orcid.org/0000-0003-3856-1682)
  * GitHub: [@krystofkomanec](https://github.com/krystofkomanec)
* **Jana Martínková** <[jana.martinkova@ds-wizard.org](mailto:jana.martinkova@ds-wizard.org)>
  * ORCID: [0000-0001-8575-6533](https://orcid.org/0000-0001-8575-6533/)
  * GitHub: [@jmartinkova](https://github.com/jmartinkova)

### Edits

* **Korbinian Bösl** <[korbinian.bosl@uib.no](mailto:korbinian.bosl@uib.no)>
  * ORCID: [0000-0003-0498-4273](https://orcid.org/0000-0003-0498-4273)
  * GitHub: [@korbinib](https://github.com/korbinib)


## Changelog

### 3.0.0

- Adjusted to template metamodel version 19.0 (released in DSW 5.0); use 2.17.x with DSW 4.x
- The template ID is now `research.data.no.questionnaire-report-lean`
- Based on upstream 3.0.0: redesigned HTML/PDF, MS Word (A4 reference document) and LaTeX formats,
  translatable texts, LaTeX output that compiles with special characters (`&`, `#`, `%`, `_` ...)
- Lean: no separate cover page (HTML/PDF), no table of contents (LaTeX), summary and history of
  versions follow the front page data
- "Selected tags" shows the question tags selected in the project (hidden if none are selected)
- Removed the organization from the front page (not part of the document context of DSW 5.0)
- Fixed project phase shown as "never" for projects without a phase or with a phase that is no
  longer in the knowledge model, and the missing current version
- Fixed empty integration answers in Markdown
- Fixed missing follow-up answers in list tables: answered follow-ups are shown inside the table
  cells; the limit of fewer than six columns counts the sub-questions and all their nested
  follow-ups, larger lists are shown as items
- Integration answers in list tables show the full value without the logo in all formats
  (LaTeX showed only the first line, HTML/PDF and Markdown the logo)
- Links to items of lists that are shown inside a table cell work in HTML/PDF
- Markdown: the summary follows the front page data and question texts are left out, as in the
  other formats
- Fixed LaTeX format that failed to render (since 2.17.1)

### 2.17.2

- Selected tags for whole questionnaire in intro
- Changed provenance 


### 2.17.1

- Tables for lists with less then 6 items, reduced whitespace
- Selected project tags moved to frontpage

### 2.17.0

- Adjusted to template metamodel version 18.0 (released in DSW 4.29.0)

### 2.16.1

- Adjusted to template metamodel version 17.1 (released in DSW 4.26.0)

### 2.16.0

- Adjusted to template metamodel version 17.0 (released in DSW 4.22.0)

### 2.15.0

- Remove External Resource Pages listing
- Improve URL to External Resource Page for LateX
- Add URL to External Resource Page for PDF/HTML, Markdown, Word

### 2.14.1

- Fixed LaTeX rendering with references

### 2.14.0

- Adjusted to template metamodel version 16 (released in DSW 4.13.0)

### 2.13.0

- Adjusted to template metamodel version 15 (released in DSW 4.12.0)
- Fixed experts
- Improved reply to value questions
- Improved resource pages
- Fixed check icon ItemSelectQuestion
- Fixed text after img for resource pages
- Fix newline in resource pages for PDF/HTML

### 2.12.1
- Reduced export

### 2.12.0

- Adjusted to template metamodel version 14 (released in DSW 4.10.0)
- Added support for item select question
- Added support for resource collections and pages (resource page references)

### 2.11.1

- Fixed nested bullet points would display unwanted characters

### 2.11.0

- Adjusted to template metamodel version 13 (released in DSW 4.3.0)

### 2.10.1

- Fixed broken images in Word

### 2.10.0

- Adjusted to template metamodel version 12 (released in DSW 4.1.0)
- Integrations should not have the link inside the item template (item URL will not be generated)

### 2.9.0

- Switched from `wkhtmltopdf` to `weasyprint` for PDF
- Improved styling for PDF and HTML

### 2.8.0

- Adjusted to template metamodel version 11 (released in DSW 3.20.0)
- Added versions overview / change tracker table

### 2.7.1

- Fixed Markdown rendering for integration question reply

### 2.7.0

- Adjusted to template metamodel version 10 (released in DSW 3.12.0)

### 2.6.0

- Adjusted to template metamodel version 9 (released in DSW 3.10.0)

### 2.5.0

- Adjusted to template metamodel version 8 (released in DSW 3.8.0)

### 2.4.0

- Adjusted to template metamodel version 7 (released in DSW 3.7.0)

### 2.3.0

- Adjusted to template metamodel version 6 (released in DSW 3.6.0)

### 2.2.0

- Using new document context

### 2.1.0

- Adjusted to template metamodel version 5 (released in DSW 3.5.0)

### 2.0.0

- Improved template visual

### 1.4.0

- Adjusted to template metamodel version 4 (released in DSW 3.2.0)

### 1.3.0

- Adjusted to template metamodel version 3 (released in DSW 2.12.0)

### 1.2.1

- Fixed issue with multiple tags on questions

### 1.2.0

- Added support for Multi-Choice questions (released in DSW 2.11.0)

### 1.1.0

- Adjusted to template metamodel version 2

### 1.0.0

- Initial version previously distributed as files directly in DSW
