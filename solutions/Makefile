SUBDIRS = 01-rotational_spectra \
          02-vibrational_spectra \
          03-line_shape \
          04-rtcalc \
          05-jacobian \
          06-olr \
          08-inversion

.PHONY: $(SUBDIRS)

subdirs: $(SUBDIRS)

$(SUBDIRS):
	@$(MAKE) -wC $@

clean:
	@for dir in $(SUBDIRS); do \
		$(MAKE) -wC $$dir clean; \
	done

cleanall:
	@for dir in $(SUBDIRS); do \
		$(MAKE) -wC $$dir cleanall; \
	done
