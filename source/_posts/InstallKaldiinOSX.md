---
title: Install Kaldi in OSX
date: 2017-08-29 17:03:31
tags:
---

I installed kaldi in my own Mac from scratch, and encountered some problems.
Here are some guidance for some one may have trouble in installing kaldi.

1. `git clone https://github.com/kaldi-asr/kaldi.git kaldi-trunk --origin golden`
2. `./kaldi-trunk/tools/extras/check_dependencies.sh`
3. Install all the dependencies. Notice that `libtoolize` is named `libtool` within `brew`.
4. `cd kaldi-trunk/tools; make`
5. `cd ../src; ./configure; make`
