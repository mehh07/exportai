# Product Vision Statement

**Project:** Historical Trends

* **FOR** historians, researchers and UVic Libraries staff who work with old Greater Victoria newspapers such as *The Daily Colonist*,

* **WHO** need to find words and topics across thousands of scanned newspaper pages, but the scans are only images and can't be searched. Reading them page by page takes far too long, and the faded, crooked print and the dense columns mixed with ads make it even harder.

* **THE Historical Trends** **IS A** web-based OCR pipeline and viewer for historical newspapers,

* **THAT** turns scanned pages into searchable text where every word keeps its exact position on the page, so a user can search a word, see every page it appears on, and jump straight to the spot on the original scan.

* **UNLIKE** browsing scans by hand or using the plain OCR text that archives usually provide (our current assumption, we still need to check which tools the library and researchers actually use today). That kind of text is often full of errors, has no word positions, and doesn't say how reliable it is,

* **OUR PRODUCT** combines a vision-language model for accurate text with Tesseract for word positions, and checks the two against each other. The VLM can invent words, so a quality score flags suspicious regions. Every output records its source file and the model that produced it, and the results use the open IIIF standard, so historians can open them in a normal viewer (Mirador) with search and highlighting.

## Notes on scope

This is an initial hypothesis. Long-term storage and hosting, and manual correction of the OCR text, are out of scope for now.
