---
title: Installation of HUGO
layout: post
guid: urn:uuid:d552da5d-5b2a-4f90-89a3-d932c71ea157
tags:
  - HUGO
  - Linux
  - BLOG
---

I found an interesting website followed the responsive web framework by [spf13](www.spf13.com). A responsive website can offer the most appropriate appearance to different terminals, such as desktop, iPad and mobile phones. You can have a look on spf13 and adjust the width of your browser window. What happened? The layout was changed to fix the width! Coooool!

The spf13 was powered by a blog system called HUGO. Umm, not come with a BOSS. I guess the "GO" means that it was developed by the famous Google GO programming language but I don't know how the "HU" came from. Anyway, I guess it is a good standing point for construct a more professional blog for planned website **MeetStuff.com**.

However, when I try to install the HUGO in my Linux desktop, I counter many minor issues which was solved gradually by asking google. I would like to mark them down here for further reference since the installation guide of official HUGO is somewhat tricky for me who is a newbie to Linux.

First, there are some dependencies of the HUGO. All of them can be install via the Ubuntu apt-get function except the Google Go. After put the Go in a proper location, there is one more step--specify the path environment.

    $ vim $HOME/.profile
    $ export PATH=$PATH:/usr/local/go/bin

Now we can check if the Go was installed correctly by running a hello world script.

Second, install HUGO.

    $ go get github.com/spf13/hugo
    $ cd ~/hugo
    $ sudo ln -s ~/hugo /usr/local/go/src/github.com/spf13/hugo

    $ go build -o hugo main.go
    $ sudo mv hugo /usr/local/bin

    $ go install github.com/spf13/hugo/hugolib
    $ go run main.go

Third, we can try to run HUGO in a server model on the sample website which is also the HUGO official website.

    $ cd /usr/local/bin
    $ hugo server --source=/home/jacobxu/hugo/docs

Then check to localhost:1313! Done!


