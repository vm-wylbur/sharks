# Authors:     PB
# Maintainers: PB, KH
# Copyright:   2017, Kaihacker, GPL v2 or later
# ============================================
# sharks/attacks/import/src/Makefile
#
all: output/import.html

# the calculation here works directly from the ipython notebook
output/import.html: \
		src/import.ipynb \
		input/GSAF5.xls.gz
	jupyter nbconvert \
		--ExecutePreprocessor.timeout=600  \
		--to html \
		--execute $<
	mv src/import.html output/

# end.
