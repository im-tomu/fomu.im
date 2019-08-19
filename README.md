# Fomu, I'm

I'm Fomu, an FPGA in your USB port!  I have 128 kilobytes of RAM, and enough logic cells to run a RISC-V CPU and a USB softcore.  I have four contact pads that can easily be used to make two buttons.  And I have an RGB LED, because everyone loves blinky things!

I'm available for [pre-order now on Crowd Supply](https://www.crowdsupply.com/sutajio-kosagi/fomu).


Developing Locally
------------------

Following the [Github Documentation on Developing Locally](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/), perform the following steps on this repo once checked out:

1. Ensure ruby is installed.  On Ubuntu/Debian, run `sudo apt install ruby ruby-dev make gcc libcurl3 autoconf libz-dev ruby-bundler`
1. `bundle install --path vendor/bundle`
1. `bundle exec jekyll serve`
