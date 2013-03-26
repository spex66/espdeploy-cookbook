espdeploy-cookbook
==================

ESPDeploy is a tool to install and customize FAST ESP solutions in a scripted and structured manner.
It is FAST ESP specific and not a direct alternative for ant or maven deployment approaches.

This cookbook is planned as a collection of configuration snippets from my years of using ESPDeploy in all of my projects.
In fact I haven't touched the ESP UI-installer since 2007, but reused my XML configuration assets over and over and shared them with my colleagues.

Maybe a bit late, but this cookbook should demystifies ESPDeploy as an 'expert' level tool.

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

Birds Eye View
==============

1) Describe your servers and services (a role like docproc, indexer, admin) in a XML file. You can have mutliple layout definitions for your stages (dev, staging, production)
2) Describe your deployment organized by tasks (like pipeline, xmlpatch, overlay) and associate them with the services

a) Install ESP based on one layout configuration
b) Patch ESP with latest Service Packs and hotfixes
c) Deploy offline customizations (ESP not started)
d) Deploy online customizations (ESP started)
