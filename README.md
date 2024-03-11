# home-pi
Using javascript and python to create a simple home finance viewer.

# Setup
### Idea: 

Make a cron job to run a python script every 30 minutes.

This script collects the past 24 hours worth of data of a handful of tickers and writes it to a .csv
I can use the yahoo finance and pandas libraries for file saving. I want to learn how to do visualisation in javascript.

Plan is to use NGINX to host a webpage, which I can update the HTML for with a javascript script.

So program flow is:

Cron job --> Python scraper --> .csv --> Javascript plot --> NGINX web server.

All in all this is pretty useless so far, but may be interesting later.

### Raspberry Pi setup
Basically just plug in some cables. Remember to supply some login info when setting things up as well as wifi info.

I prefer doing development via SSH in VS Code, so chose a headless OS for my pi for increased performance.

### Python installation

Turns out, you can just make a venv somewhere in a folder for this project, if the out-of-the-box python
is new enough for you. You can also just specify a higher python version for the venv if needed.

You can make your venv with:

```
python -m venv website-proj
```

Then you can do the usual `source some-path-here/website-proj/bin/activate`.

### Javascript installation
