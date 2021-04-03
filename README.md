# Chromatic co-occurrence of local binary pattern (CCoLBP) for face presentation attack detection (aka face anti-spoofing or spoofing detection)

Table of Contents
=================

- Introduction
- Usage
- Additional information
- Contact

Introduction
============

This source code provides a simple implementation of intra-channel and inter-channel based descriptors in face PAD. It includes the CCoLBP and the block based LBP. It is very easy to use and reproduce our work.

Usage
=====

The two core functions of this implementation

a) For the CCoLBP

Example:

F = CCoLBP(I, s, r, config, mode);	% such as F = ColorCoALBP(I, 1, 2, 1, 'h');
	
This example returns the CCoLBP of the input image. Other parameters are described in CCoLBP.m.

b) For the block based LBP

Example:

lbp_blk = lbp_blk(I, lbp_r, lbp_p, mappingtype, mode, rowstep, colstep);	

% such as blklbpfea = lbp_blk(I, 1, 8, 'u2', 'h', 32, 32);

This example returns the block based LBP of the input image. Other parameters are described in lbp_blk.m.

Additional information
======================

The implementation of LBP is licensed to Timo Ojala, Matti Pietikainen, and Topi Maenpaa,
[1] T. Ojala, M. Pietikainen, and T. Maenpaa,
    "Multiresolution gray-scale and rotation invariant texture classification with local binary patterns,"
    IEEE Transactions on Pattern Analysis and Machine Intelligence, vol. 24, no. 7, pp. 971–987, Jul. 2002.

The implementation of CCoLBP is licensed to Peng Fei, Qin Le, and Long Min, 
College of Computer Science and Electronic Engineering, Hunan University, Changsha, China.
College of Computer and Communication Engineering, Changsha University of Science and Technology, Changsha, China.
