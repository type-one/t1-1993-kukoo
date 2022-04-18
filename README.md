What
----

Text Mode BBSTro
Released January 1993
MS-Dos

https://demozoo.org/productions/142609/

KUKOO - An Advertising Intro for -= Pleasure Access BBS =-

9.5k ASM pure juice !!! pure VGA Text mode (82x29) ...

Old skool MS-DOS text mode bbs-tro running on VGA and 286/20 mhz  

It was running on 90's VGA cards like Cirrus Logic, ATI, S3, Trident.
The typical VGA graphic cards you had on 286/386 MS-DOS computers at that time.

I had a Trident VGA card in an ISA slot at that time and I was experimenting with
VGA card registers, inspired by tricks I was playing on my Atari ST.

The intro itself is a 16-bit executable using Intel 286 instructions.
It uses an expanded Text Mode of 82x29 (fullscreen) instead of the standard 80x25.

The intro was published beginning of 1993 on some Belgian BBSes and on some FTP 
sites that were popular in the early 90-ties (ftp.oulu.fi, hornet, ...).  
It was mirrored later on sites like scene.org.

Most of the code was started and written during autumn/winter 1992, the year
I started Computer Sciences at the University and when I left my Atari ST
for the PC, upgraded from a 286/20 mhz to a 486/33 mhz motherboard.  It was
also the first year of my life where I did have access to the Internet as 
a student.

The released intro was compressed using PKLITE (from what I remember)

http://fileformats.archiveteam.org/wiki/PKLITE

The source is a single x86 assembly language file (.ASM) that includes some precomputed tables and some assets
converted into asm data.  A lot of comments in the code are in french, with some private jokes that only a few
friends who were studying with me will understand ;-)

Build
-----

To build the executable you will need a MASM compatible assembler with a 16 bit linker.

Use Windows and run **build.bat** in the src folder.

One possibility is to use the legacy MASM assembler that Microsoft released for free a decade ago.

Another is to use the free compatible JWasm assembler available here: 

https://www.japheth.de/JWasm.html

Instructions to use MASM 6.14 and LINKER 5.63 are available here:

https://service.scs.carleton.ca/sivarama/asm_book_web/free_MASM.html

http://www.masm32.com

Microsoft's MASM 6.14 is included in the masm32 package.

To get MASM 6.14, download masm32V8.zip from:

http://www.masm32.com/ (2.98 MB)

Unzip and run install.exe. It creates masm32 directory. 
The MASM files (ml.exe and ml.err) are in the masm32/bin directory.

Do NOT use the linker link.exe (32 bit) in the masm32/bin directory. 
Use the linker version 5.60 to generate 16-bit DOS applications. 

You can get this by googling for "Microsoft BASIC Softlib Collection"

Execute lnk563.exe to extract link.exe file.

You need these three files (ml.exe, ml.err, and link.exe) to run the assembly programs. 

You can just drop these 3 files in the src folder or copy the **jwasm.exe** executable there.


Run
---

On **DosBox** you have to use machine=vgaonly in the emulator settings

On real MS-DOS PC with MS-DOS 6.2+, an AdLib compatible card (SoundBlaster, SoundBlaster Pro, SoundBlaster 16, AWE32/64)
and an ISA/VESA VGA card or some older PCI VGA cards (like S3 Trio, S3 Virge).

I still achieve to run it on my old (preserved) 486 DX2-66/S3 (1995) and a K6-2 500/S3 Virge DX (1999), that are still working 
today in 2022.

