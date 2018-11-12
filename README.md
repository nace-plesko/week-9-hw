# week-9-hw

Which Honeypot(s) you deployed

  I deployed Ubunut-Dionaea with HTTP
  
Any issues you encountered

  I had some issues with setting up the environment. In particular, when I was trying to use zone us-central1-c on GCP as it is instructed in the lab writeup, it didn't work. Then I used us-east4-c and it solved the problem. The second issue I had was with running sudo ./install.sh, because github repo from which it was installing was changed apparently, so I had to edit the install_hpfeeds.sh file and change the line pip install -e git+https://github.com/HurricaneLabs/pyev.git#egg=pyev to pip install -e git+https://github.com/couozu/pyev.git#egg=pyev. Thankfully it didn't took me too long to figure it out, because someone else posted this issue already on piazza.
  
A summary of the data collected: number of attacks, number of malware samples, etc.

  In the last 24 hours there were 4362 attacks, the most attacked port was 8088, it seems like it's a common vulnerable port (it was attacked roughly 8x more than the second most attacked port). I can see that there were attacks pretty much from all around the world, which is really concerning and it shows that internet is not a safe environment at all.
  
Any unresolved questions raised by the data collected

  Since I got plenty attack already right after I deployed a honeypot, I am wondering if there are servers all around the world scanning the internet all the time and looking for vulnerable sites in order to take the advantage of them right away.
