Introduction
============

In the summer of 1994, I graduated from the University of Sheffield with my Batchelor's Degree in Software Engineering, and was then hired by the university to work on a national research project looking at UNIX batch processing systems.  My role was to take the Network Queueing System (NQS)software, port it to the UNIX systems commonly used at universities around the UK, and to improve its reliability.

It was to prove to be a baptism of fire in the art of creating robust software.

Back in the mid-1990s, desktop PCs weren't very powerful, and computational scientists were forced to run the calculations for their experiments on large, centralised UNIX computers that were often shared across whole departments or universities.  These calculations could take days, weeks or sometimes months to run.  Batch processing systems like NQS were used to manage the queueing and execution of these calculations, and if they crashed, the calculations often had to be restarted from the very beginning.

NQS was originally developed under contract for NASA in the 1980's, but unfortunately it wasn't as solid a piece of software as it needed to be.  The Monsanto Company acquired rights to NQS and oversaw improvements to it, as did CERN and several companies.  Monsanto released their improvements on the Internet under the GNU General Public License. It was my job to support and enhance Monsanto-NQS further.

Like most software that was written for UNIX back then, NQS was written in C.  C is one of those languages that you either love or hate.  It allows the programmer to write code that's very close to how the underlying CPU instructions work, but it's also abstracted just enough from those instruction sets to make it relatively easy to port code from one UNIX variant to another.  On the flip side, C's tremendous power makes it an unforgiving language to program in, and it's not easy to write C code that is robust enough to survive the rigours of regular use.

I spent twenty months working for the University, and afterwards continued to maintained the now-renamed Generic NQS software up until the late 1990's.  During that time, I ported NQS to over twenty UNIX variants, and worked on turning it into a solid and dependable piece of software.  Much of this work relied heavily on email correspondance with its users around the world, and at the start was very much trial and error.  I made many mistakes along the way, as I figured out how to improve not only NQS, but also how to improve my own approach to developing and supporting software over the Internet.

Today, NQS isn't even a footnote in history - there's no Wikipedia entry for it, although you can still find a copy of the source code on SourceForge - and it has been superceeded first by Grid Computing and then by Cloud Computing.  Most programmers no longer work in C, but instead use higher-level languages such as Java or PHP, where so much of the lower-level detail is handled for them by the languages' runtime environments.

And yet, the lessons from nearly 20 years ago are needed just as much today.  Buggy software costs, whether it is the computational scientist who has lost two months time in his research, or the web app business who keeps disappointing customers and losing reputation and revenue.

I've spent all of my career applying those lessons to every organisation I've worked for.  In this book, I'm going to show you what I do to create robust software in PHP, and why, in the hope that it'll help you to choose your own practices for doing so too.