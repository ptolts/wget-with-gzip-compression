wget-with-gzip-compression
==========================

I was looking for wget with gzip support. I found this version https://github.com/kravietz/wget-gzip which appeared to do what I wanted, but it was Windows only. I used that code as inspiration and implemented it in the latest version of wget. It works, but it's ugly. I don't bother checking if the returned page is actually compressed, I just open it with gz_open and then save it again. It works though!


This was done in a few hours. I don't code in C regularly, and I have to move onto other stuff now. To compile this, I run ./configure and then I manually add "-lz" to the LIBS variable in the Makefile. Someday I'll get around to learning how to configure configure.
