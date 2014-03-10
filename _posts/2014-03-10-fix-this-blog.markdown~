---
title: 重新弄好了這個blog
layout: post
guid: urn:uuid:9a90ae04-e1dc-4f99-8283-5b412ee92f92
tags:
  - 
---

好久沒有更新這裏了。在換成了Linux系統之後，很長一段時間都懶得去重新設定jekyll和github，今天沒有出門閒到蛋疼就無意中想起這裏，鼓搗了一下。

發post的命令備忘


	rake post[testing]
	
	git add .
	git commit -m "testing"
	git push origin master



{% highlight r %} par(bg = "black", mar = rep(0, 4), pch = 20) xx = runif(100) yy = runif(100) plot(xx, yy, type = "n") mousemove = function(buttons, x, y) { r = 0.2 idx = (x - r < xx & xx < x + r) & (y - r < yy & yy < y + r) plot(xx, yy, type = "n") rect(x - r, y - r, x + r, y + r, border = "yellow", lty = 2) points(xx[idx], yy[idx], col = "yellow", cex = 2) points(xx[!idx], yy[!idx], col = "red") NULL } mousedown = function(buttons, x, y) { "Done" } getGraphicsEvent("Click mouse to exit", onMouseDown = mousedown, onMouseMove = mousemove) {% endhighlight %}
