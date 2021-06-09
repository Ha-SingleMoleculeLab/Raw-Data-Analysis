# Raw-Data-Analysis

PMA files recorded by Single should be “analyzed” to get the smFRET traces of molecules recorded in the PMA files. The “analysis” is done with IDL (Research Systems, Inc.), and this manual documents how to use the group of IDL scripts written for PMA file analysis. 


The scripts documented here assume the followings.

•	.PMA files have more than 12 frames
•	.PMA files have a pixel resolution of 512 by 512
•	The left half of a frame, [1, 256] x [1, 512], is the donor channel, and the right half, [257, 512] x [1, 512], is the acceptor channel.
•	The width and the height of a pixel of the .PMA files are ~ 100nm. (The physical dimension of a pixel of typically used Andor cameras is 16um by 16um, and the magnification by a microscope and optics is 150X. ref. Selvin, P.R. and T. Ha, Editors, "Single Molecule Techniques: A Laboratory Manual", Cold Spring Harbor Laboratory Press ISBN 978-087969775-4 ) 


The scripts were last updated back in 2000. Thus, somewhat old versions of IDL should work with them. In our case, IDL Student Edition 6.2 is working fine.
