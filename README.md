# amiga-ptplayer-minimal
This is a  modified version of Frank Wille's ptplayer Amiga Protracker replay source with changes for small / 64KB demo productions to reduce the size of the code in the executable.

The original code is on Aminet: http://aminet.net/package/mus/play/ptplayer

The changes are:
* mt_data is in BSS (no longer completely PC relative, focused on exe size) 
* MINIMAL_ENABLE_VIB_SAWRECT to enable SAW and RECT vib/tremolo. Saves a few KB.
* Period table generated in code saving about 1KB.
* VUMeter trigger added in _mt_VUMeter

Jonathan Bennett / Antiriad
