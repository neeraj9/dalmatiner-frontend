VERSION=0.3.3
COMPONENT_INTERNAL=dfe
COMPONENT=dalmatinerfe
DEPS="erlang" "coreutils" "sudo"

include ../../_build/default/lib/fifo_utils/priv/pkg.mk

.PHONY: prepare

prepare:
	-rm -r $(STAGE_DIR)/$(COMPONENT)
	cp -r ../../_build/${REBARPROFILE}/rel/$(COMPONENT_INTERNAL) $(STAGE_DIR)/$(COMPONENT)

package: prepare $(FILE).tgz

clean: clean-pkg
	-rm *.tgz

