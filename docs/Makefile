# Minimal makefile for Sphinx documentation
SPHINXOPTS    ?=
SPHINXBUILD   ?= sphinx-build
SOURCEDIR     = .
AUTOSOURCEDIR = $(SOURCEDIR)/modules
BUILDDIR      = _build

# Put it first so that "make" without argument is like "make help".
help:
	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)

.PHONY: help all clean-apidoc Makefile

all: clean clean-apidoc html

clean-apidoc:
	rm -rf "$(AUTOSOURCEDIR)"

# Catch-all target: route all unknown targets to Sphinx builder
%: Makefile
	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
