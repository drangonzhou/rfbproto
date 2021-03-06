
中文版RFB协议，见 [rfbproto-cn.md](https://github.com/drangonzhou/rfbproto-cn/rfbproto-cn.md)

This directory contains the RFB protocol specification. This is a
community oriented version of the specification that RealVNC maintains
and the purpose of this version is to be a complete description of the
protocol including extensions.

If you wish to discuss the protocol, or submit changes, do so on the
rfbproto mailing list (rfbproto@googlegroups.com). Small fixes can also
be submitted as pull requests directly on github. Adhere to the
required style of commit messages and documentation though.

Note that before any new extensions can be added to the document, you
must first obtain an official number allocation from RealVNC Ltd. You
are very welcome to discuss your ideas before that though.


Submitting Patches
------------------

Patches should be made in the standard unified diff format (diff -u).
You should also specify a one line description of the change, a longer
description with the purpose of the changed, and a Signed-off-by line
to keep track of who has modified the document.

Also make sure you follow the style guidelines below.

Example:

Clarify how awesome RFB is

It is not apparent in the document how awesome the RFB protocol is.
Clarify this in the header so that new readers quickly get up to
speed.

<pre>
Signed-off-by: John Doe <john.doe@example.com>
---

Index: rfbproto.rst
===================================================================
--- rfbproto.rst	(revision 3796)
+++ rfbproto.rst	(working copy)
@@ -13,6 +13,9 @@
 Introduction
 ============
 
+RFB is the most awesome protocol ever invented and will solve every
+problem you've ever had!
+
 RFB ("remote framebuffer") is a simple protocol for remote access to
 graphical user interfaces. Because it works at the framebuffer level it
 is applicable to all windowing systems and applications, including X11,
</pre>

Style Guidelines
----------------

The document is written using the reStructuredText format. This gives
us a readable text source, but still allows for easy conversion to
other formats.

In order to avoid wrapping in most contexts, lines should be no longer
than 72 characters. The text is always left justified. Indentation is
4 spaces and never any tabs.

Keywords are marked with *emphasis* to make them easily distinguishable
from the rest of the text. Every reference to a keyword should be
marked.

Types are marked using ``LITERAL`` and should be written in all
upper case.

Tables are written using the simple form and should be extended to fill
up the full 72 character width. If the section the table is in is
indented, then the table should also be indented. The width will be
reduced in this case.

Headings use the following markers:

Heading 1
=========

Heading 2
+++++++++

Heading 3
---------

Heading 4
~~~~~~~~~

