wget-with-gzip-compression
==========================

I was looking for wget with gzip support. I found this version https://github.com/kravietz/wget-gzip which appears to do what I wanted, but it was for Windows. I used that code as inspiration and implemented it in the latest version of wget. It seems to be working, but its ugly. I don't bother checking if the returned page is actually compressed, I just open it with gz_open and then save it again. It works though!
