# Atom Knowledge Base

Back when my job had me using a Macbook, I picked up a copy of Devonthink Pro and was immediately fascinated by the idea of keeping a database to collect and organize the knowledge I filter through on a daily basis. Unfortunately, the OS limitations kept me from using it to its full potential, and when I switched jobs I never really replaced it. I've made do with collections of PDFs in Google Drive, notes in OneNote, and repositories here and there for writing projects.

There are a few open-source notebooks, wikis, etc. that are sometimes billed as replacements for Devonthink, but many were missing features I'd like to have, and none really jumped out at me. I considered developing my own, but it occurred to me that it might be easier to build a toolchain of components that can give me the functionality I'm after.

## Key Objectives

**Collection.** I want to pull in data from a variety of sources: web pages that I'm browsing, PDFs I am reading, notes I generate on the fly, captured screenshots, or other documents (of any type). I'd also like the option to pipe data in automatically via APIs.

**Synchronization.** I want to have access to the same data on my laptop, desktop, and optionally mobile (tablet or phone).

**Editing.** I want notes to have, at a minimum, simple formatting; hyperlinks, to local files or web URLs; and embedded images.

**Organization.** I want to search for information across file types, in text notes, PDFs, perhaps even images (with OCR). I want to be able to organize files and documents by folders, at least, and optionally by tags or other metadata as well.

## Atom as an Anchor

I want a flexible editor with a powerful plugin system to anchor this knowledge base. The less we have to rely on external applications, the better. I considered Visual Studio Code initially, but it had no way to effectively embed a proper browser tab. Atom does have those extensions, and better markdown handling, so that is where I settled.

# The Build

As noted above, the core of the build is the Atom editor. 

## Atom Extensions

I've added the following extensions:

* markdown-writer: Nicer handling of markdown notes
* markdown-image-assistant: Ability to drag/paste images directly into markdown (saving the image beside the markdown file, and adding the image reference)
* inline-markdown-images: Display referenced images inline in the markdown notes (so we don't need to preview our markdown just to see the images)
* pdfjs-viewer: Open PDFs within Atom
* hyperclick and hyperclick-markdown: Enabling ctrl+click for hyperlinks in markdown
