# amiga-ptplayer-minimal
This is a  modified version of Frank Wille's ptplayer Amiga Protracker replay source with changes for small / 64KB demo productions to reduce the size of the code in the executable.

The original code is on Aminet: http://aminet.net/package/mus/play/ptplayer

The changes are:
* mt_data is in BSS (no longer completely PC relative, focused on exe size) 
* MINIMAL_ENABLE_VIB_SAWRECT to enable SAW and RECT vib/tremolo. Saves a few KB.
* Period and finetune table generated in code saving about 1KB.
* Vibrato sine table generate in code saving about 1KB.
* VUMeter trigger added in mt_VUMeter which allows for demo/music sync effects with playing notes

Jonathan Bennett / Antiriad
