# Chromatic co-occurrence of local binary pattern (CCoLBP) for face presentation attack detection

Peng F, Qin L, Long M. CCoLBP: Chromatic Co-Occurrence of Local Binary Pattern for Face Presentation Attack Detection[C]//2018 27th International Conference on Computer Communication and Networks (ICCCN). IEEE, 2018: 1-9. DOI: 10.1109/ICCCN.2018.8487325

Paper (conference version): https://ieeexplore.ieee.org/abstract/document/8487325

Peng F, Qin L, Long M. Face presentation attack detection based on chromatic co-occurrence of local binary pattern and ensemble learning. Journal of Visual Communication and Image Representation, 66, 102746. DOI: 10.1016/j.jvcir.2019.102746

Paper (journal version): https://www.sciencedirect.com/science/article/abs/pii/S1047320319303670

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
