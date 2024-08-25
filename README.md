# NHocr

OCR Engine for Japanese

Since Sep 8, 2008 (at Google Code) / Repository at GitHub opened on Aug. 25, 2024  
Last update: Aug. 25, 2024

## Introduction
NHocr is a command line OCR (Optical Character Recognition) program for Japanese, Chinese, etc. It has been designed to recognize machine-printed Japanese characters and some ASCII characters/symbols in an image.
NHocr is probably the first Open Source Japanese OCR software (offline, machine-printed), except some experimental, partial codes open to academic communities.

You can also use NHocr through WeOCR service at:
 * https://maggie.ocrgrid.org/nhocr/

The program is highly experimental, and the character recognition performance is limited.
You would become happier with a commercial product if you want a high performance OCR.
Recent OCR libraries such ``Microsoft OCR Library for Windows Runtime''
are also useful (and perform better).

The character feature used in NHocr is based on Peripheral Local Moment (P-LM) proposed by Hori et al. in late 90s.

Please don't expect too much.
This software was developed before the Deep Learning 
and LLM (Large Language Models) era. 

**This is here just for a historical record.**

NHocr is originally a product of the author's weekend programming. The development work may be rather slow.


## Changes of the repository

The project site was originally hosted by Google Code.

Since Google suddenly discontinued the service, 
the source package repository was changed to SourceForge .JP (OSDN).
However, the operation of SourceForge .JP went wrong, and the site
contents were lost.

Now, NHocr repository is here at GitHub 
although the development is suspended (almost?).


## Limitations of the current version

 * The current NHocr can handle text block image only, since it has not been equipped with a page layout analysis engine.
 * The recognition accuracy may deteriorate when wide and narrow characters are mixed or when proportional fonts are used.
 * The character segmentation performance is limited, since a primitive segmentation algorithm is used in the current version.
 * The recognition accuracy with ASCII characters may not be so good. Using another OCR, such as tesseract, is recommended for European languages.
 * The language post-processor "gramd" is experimental and works with Japanese text only. Some side effects may exist.



## Supported platforms and requirements
Solaris SPARC/x86 and Linux are officially supported.
NHocr would work on other UNIX(-like) platforms and MS-Windows.

NHocr uses FreeType 2 available at:
 * https://www.freetype.org/

## Supported languages
The current version of NHocr supports Japanese and Chinese.

The author is interested in supporting other oriental languages such as Traditional Chinese. Character code table cctable-xxx is required. Contributions are welcome.

## License
Apache License 2.0

