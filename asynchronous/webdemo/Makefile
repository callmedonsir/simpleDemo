# Copyright 2009 The Go Authors.  All rights reserved.
# Use of this source code is governed by a BSD-style
# license that can be found in the LICENSE file.

include $(GOROOT)/src/Make.inc

TARG=webdemo
GOFILES=\
	timer.go\
	data.go\
	page.go\
	async.go\
	sync.go\

CLEANFILES+=webdemo

include $(GOROOT)/src/Make.pkg

%: install %.go
	$(GC) $*.go
	$(LD) -o $@ $*.$O

run: webdemo
	./webdemo
