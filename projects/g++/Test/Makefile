.PHONY: release debug clean clean-release clean-debug install

DIRS:= ../build ../build/test

all: $(DIRS) test 

$(DIRS):
	mkdir $@

clean:
	( cd ../build/test && $(MAKE) --no-print-directory clean )


#release:
#	( cd build/release && cmake -DCMAKE_BUILD_TYPE=release ../.. && $(MAKE) --no-print-directory && make  --no-print-directory install)
#	ctags -R  --language-force=c++ *.*
#	ctags -eR  --language-force=c++ *.*
