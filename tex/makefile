island.pdf: island.ps
	ps2pdf $< 
	#ps2pdf $< && cp cycle.pdf cycle.1.pdf
island.ps:island.dvi
	dvips $<
island.dvi: island.tex  
	latex $< && latex $<

ifdef COMSPEC
# in windows
include ..\..\clean.mk
else
include ../../clean.mk
endif
