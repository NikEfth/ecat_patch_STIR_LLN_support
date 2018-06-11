# Ecat patch for LLN support for STIR
This is a patch to apply in the ecat library, usually downloaded from [OpenGateCollboration](http://opengatecollaboration.org/ECAT "OpenGateCollaboration"), in order to be able to complile [STIR](http://stir.sourceforge.net/) with LLN support. 

For information and reasoning on the nessesity of this patch please refer to [this](https://github.com/UCL/STIR/issues/207 "Linking to libecat fails (Arch linux 2018.05.15) #207") discussion on github, issue #207. 

[This](http://stir.sourceforge.net/wiki/index.php/STIR_FAQ#Problems_with_ecat_library "STIR FAQ") wiki page provides instruction on how to install the patch. Briefly, 

1. Go to the local ecat directory (before compilation)
2.  Move the patch file to the directory of the original folder 
3.  This folder will get modified, so make a backup of it somewhere 
4. Run: 

```bash
patch -s -p0 < stir_ecat_no_rts_no_xdr.patch
```

5. At this point, the original folder contains the modified content. 



*Good luck with your reconstructions!*