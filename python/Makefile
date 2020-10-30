SUBDIRS = sepolicy audit2allow semanage sepolgen chcat

all install clean:
	@for subdir in $(SUBDIRS) po; do \
		(cd $$subdir && $(MAKE) $@) || exit 1; \
	done

relabel indent test:
	@for subdir in $(SUBDIRS); do \
		(cd $$subdir && $(MAKE) $@) || exit 1; \
	done
