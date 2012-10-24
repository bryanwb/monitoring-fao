<!SLIDE center>

<center style="font-size:6em;">
Monitoring data.fao.org
<br /><br />
</center>
![alt text](preso-front1.png)
<br />
KISAF Presentation October 23, 2012, Bryan W. Berry

!SLIDE
# Ohai There

*  I am in charge of infrastructure for the [http://data.fao.org](http://data.fao.org) project
* In free-time, I am creator and co-host of the
  [Food Fight podcast](http://foodfightshow.org)
<br /><br />
<div style="float:left;">
<img src="data-fao-org-logo-v8-bigger.png"></img> &nbsp; &nbsp;
<img src="foodfight_banner.png" width="250px" height="105px"></img>
</div>

!SLIDE
# more on data.fao.org

<img src="screenshot01.png" height="480px" width="500px"></img>

!SLIDE 
# Overview

* SOA is complicated
* Monitoring Helps
* But What does it all mean?
* How you can start monitoring your applications
* Show me the Math!

!SLIDE full-page
# data.fao.org Architecture on Paper 

<center>
<img src="data_fao_org_arch.jpg"></img>
</center>

!SLIDE full-page

<center><img src="spaghetti-bolognese.jpg" height="900px" width="700px" /></center>

<center style="font-size:3em;">The Reality</center><br />

.notes http://dummyatcooking.files.wordpress.com/2007/10/spaghetti-bolognese.jpg

!SLIDE
# What We use for Monitoring

* Collectd (cpu, disk, network, arbitrary system data)
* JMXtrans to poll JMX data
* Logstash + statsd awesome combination
* Graphite
* Elasticsearch + Kibana


largely based on discussion in [foodfightshow episode 21](http://foodfightshow.org/2012/07/monitoring-for-n00bs-with-jason-dixon.html)

!SLIDE 
# Here is what it looks like
<center>
<img src="full_stack.png"></img>
</center>

!SLIDE
# Let There Be Graphs!

<center>
<img src="moar_graphs.png"></img>
</center>

!SLIDE
# Graphite Demo

<center style="font-size:4em;">
        <a href="http://graphite.data.fao.org">
        <div style="text-decoration:blink;">
        http://graphite.data.fao.org
        </div>
        </a>
</center>

!SLIDE
# Monitoring changes how you work

<center>
<img src="deming-quality.jpeg.jpg"></img>
</center>

<center style="font-size:3em;">
    <em>
    In God we trust, <br />
    All others must bring data
    </em>
</center>
<center>
W. Edwards Deming
</center>

!SLIDE
# Don't be a Phenomonologist, Be a Scientist
    
<center>
<img src="phenom_or_scientist.png"></img>
</center>

!SLIDE
# Do you know What this means?

<img src="request_latency-svg.png"></img>

Just collecting the data isn't enough

!SLIDE
# How fast/slow is the site?

* How many Requests per Second? Per minute?
* Are those thousands of seconds or thousands of milliseconds?
* What is the average request latency?
* Is "average" what we really want to know?


!SLIDE full-page
<center>
<img src="confusing_graphs.png"></img>
</center>

.notes http://www.buzzlol.com/wp-content/uploads/2012/05/Confused-Dog-Is-Confused.jpg
