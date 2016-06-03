## WordPress Cluster

This repository provides [WordPress Cluster](http://www.wordpress.org/) JPS-based installation package for Jelastic Platform.

**WordPress Cluster** is highly available and scalable clustered solution for WordPress, the extremely popular open source CMS and blogging tool.

**Engine**: PHP 5.4.0

### Environment Topology

![Wordpress Cluster Topology](https://docs.google.com/drawings/d/11pvt6b_5t8Vscqruzl3KRhp8u883TKEwUFio8UrDDGk/pub?w=269&h=383)

Layer                |   Server  | Number of nodes   |  Cloudlets (reserved/flexible)  |  Specifics
-------------------- | --------- | :---------------: | :-----------------------------: | :---------:
Load Balancing       |  NGINX LB |       2           |           2 / 16                | with [external IP](https://docs.jelastic.com/public-ipv4) address 
App Server           | NGINX-PHP |       2           |           2 / 32                | -
SQL database         |    MySQL  |       2           |           2 / 16                | -

### What it can be used for?
This package is designed to ensure the load tracking and distribution, as well as automatic adjusting the amount of allocated resources according to it.<br />
WordPress can be used to create a beautiful website, blog, or app. This web application is both free and priceless at the same time.
WordPress started as just a blogging system, but has evolved to be used as full content management system and so much more through the thousands of plugins and widgets and themes, WordPress is limited only by your imagination. (And tech chops.)<br />

In order to get this solution instantly deployed, specify your Jelastic account email address and choose the required platform within the widget below:

![GET IT HOSTED](https://raw.githubusercontent.com/JelasticJPS/jpswiki/master/images/getithosted.png)

For more information on what Jelastic JPS package is and how to install it, follow the [Jelastic JPS Application Package](https://github.com/JelasticJPS/jpswiki/wiki/Jelastic-JPS-Application-Package) reference.
