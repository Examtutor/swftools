# swftools
SWFTools-0.9.2

gif2swf errors during compilation due to giflib is now corrected

How to install in ubuntu 16.04 LTS

sudo apt-get install build-essential checkinstall
sudo apt-get install libgif-dev xpdf libfreetype6 libfreetype6-dev libjpeg62 libjpeg8 libjpeg8-dev

Download this repository to /tmp folder
unzip the file
./configure
make

Edit /swfs/Makefile to comment the following 2 lines (to look something like below, note # beginning of the line)
#rm -f $(pkgdatadir)/swfs/default_viewer.swf -o -L $(pkgdatadir)/swfs/default_viewer.swf 
#rm -f $(pkgdatadir)/swfs/default_loader.swf -o -L $(pkgdatadir)/swfs/default_loader.swf

sudo checkinstall

Insert the name of the package (SWFTools) when prompted by checkinstall and follow the procedure as usual.
