Please join the discussion about this project on LinkedIn 'FAST ESP' group and share your feedback. 

What feedback? 
* Can you follow this steps?
* Your interest and use cases in more chapters (I want write for my own, but for your benefit :))

Thank you

espdeploy-cookbook
==================

ESPDeploy is a tool to install and customize FAST ESP solutions in a scripted and structured manner.
It is FAST ESP specific and not a direct alternative for ant or maven deployment approaches.

This cookbook is planned as a collection of configuration snippets from my years of using ESPDeploy in all of my projects.
In fact I haven't touched the ESP UI-installer since 2007, but reused my XML configuration assets over and over and shared them with my colleagues.

Maybe a bit late, but this cookbook should demystifies ESPDeploy as an 'expert' level tool.

Go for the Wiki pages and check the recipes out.
Please give feedbacks on your experiences with that recipes and for which of your real world use-cases you want to have a recipe.


History
=======
Initially it was programmed by FAST Professional Services for Professional Services to ease the day to day work.
It is written in Python 2.3, but not Open Sourced by Microsoft. 

Prerequistes
============
So you need to have a Microsoft Connect account to get access to the latest ESPDeploy binaries for Linux or Windows.

Documentation
=============
ESPDeploy isn't the best documented tool, because it never reached a product status. 
But with every project delivered, we documented and trained our customers how to use ESPDeploy for:
* repeated installations to various server topologies (single, three nodes, 80 nodes)
* disaster recovery scenarios
* Maintenance upgrades (Hotfixes, SP, index-profile, additional nodes, code changes, etc...)

Bird's Eye View
==============

1. Describe
  * Describe your servers and services (a role like docproc, indexer, admin) in a XML file. You can have mutliple layout definitions for your stages (dev, staging, production)
  * Describe your deployment organized by tasks (like pipeline, xmlpatch, overlay) and associate them with the services
2. Execute
  * Install ESP based on one layout configuration
  * Patch ESP with latest Service Packs and hotfixes
  * Deploy offline customizations (ESP not started)
  * Deploy online customizations (ESP started)
 

