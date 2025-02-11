---
layout: page
category: walkthrough
title: Sequencing tutorial
is-detailed: true

---

<video controls>
    <source src="presentations/miso_sequencing.mp4" type="video/mp4">
</video>

[Download the PDF]({{ '/presentations/miso_sequencing.pdf' | prepend: site.baseurl }})



<div id="toc">
Table of Contents
<ol>
   <li><a href="#logging_in">Logging In</a></li>
   <li><a href="#uorders">Checking for unfulfilled Orders</a></li>
   <li><a href="#sequencing-pool-orders">Working with Pool Orders</a></li>
   <li><a href="#runs-new">Creating Runs from scratch</a></li>
   <li><a href="#runs-auto">Working with automatically created runs</a></li>
   <li><a href="#runs-add-pools">Adding Pools to Runs</a></li>
   <li><a href="#runs-qcs">Mark a library as Low Quality</a></li>
   <li><a href="#boxes">Scanning libraries into your outbox</a></li>
   <li><a href="#service-records">Adding Service Records to Instruments</a></li>
   <li><a href="#runs-trouble">Troubleshooting</a></li>
</ol>
</div>

<div id="infobox">
Print the worksheet for this section here: <a href="worksheet-detailed-sequencing">Sequencing Worksheet</a>.
</div>

{% include logging_in.md detailed=page.is-detailed %}

{% include uorders.md %}

## 2.1 Scan pools into your inbox

First, scan the pools from the libraries team into your inbox for further work.

{% include inboxes.md %}

{% include sequencing-pool-orders.md detailed=page.is-detailed %}

{% include runs-new.md section=4 flowcell=site.flowcell sequencer=site.sequencer
  platform=site.platform platform_type=site.platform_type seq_params=site.seq_params %}

{% include runs-auto.md %}

{% include runs-add-pools.md detailed=page.is-detailed %}

{% include runs-qcs.md %}

<a name="boxes" href="#" id="toplink">top</a>

# 7. Scanning libraries/pools into your outbox

{% include outboxes.md %}

{% include service-records.md %}

{% include runs-trouble.md %}

< <a href="tutorial-detailed-libraries">Libraries</a> | <a href="index">Home</a> | <a href="tutorial-detailed-index-distance">Checking Index Distance</a> >
