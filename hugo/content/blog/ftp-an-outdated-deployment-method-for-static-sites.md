---
title: 'FTP: An Outdated Deployment Method for Static Sites'
description: ''
date: 2019-01-15 22:57:29 -1100
authors:
- Sebastian Engels
publishdate: 2019-01-16 07:00:00 -1100
expirydate: 2030-01-01 04:00:00 +0000
categories:
- CMS
headline: ''
textline: ''
images: []
tags: []
cta:
  headline: ''
  textline: ''
  calls_to_action: []
private: false
weight: ''
aliases: []
menu: []
draft: true

---
{{% warning %}}

Current users of the FTP deployment method are able to continue to use FTP for the foreseeable future. However, we won't add any additional features or output and we truly believe that you should switch to a more secure deployment method such as SFTP (SSH-based deployment).

{{% /warning %}}

A lot has been said on the security vulnerabilities of plain FTP already. [This](https://www.ssh.com/ssh/ftp/server), [this](http://blog.jdpfu.com/2011/07/10/why-you-need-to-stop-using-ftp) or [this](https://www.motherjones.com/politics/2017/10/trump-election-commissioners-voter-database-is-a-ripe-target-for-hackers/) and [the list goes on](https://www.google.com/search?q=ftp+security+issues&oq=ftp+security+issues&aqs=chrome.0.69i59j0l4.3491j0j4&sourceid=chrome&ie=UTF-8). FTP hasn't been secure since the mid-1990s but Forestry has supported it until now as it is often an easy way to kick the tires and get started with a demo or test site.

The simplicity of FTP is certainly its biggest selling point but even easier ways to host and deploy your sites has emerged and they are gaining rapid adoption in the developer community. That's why we believe it is time to lay FTP-support to rest and stop letting people board this train to no-man's-land.

<div style="width:100%;height:0;padding-bottom:46%;position:relative;"><iframe src="https://giphy.com/embed/Az1CJ2MEjmsp2" width="100%" height="100%" style="position:absolute" frameBorder="0" class="giphy-embed" allowFullScreen></iframe></div>

## We'll let FTP die

Forestry will stop supporting FTP, FTP with Implicit SSL and FTP with TLS/SSL starting **XX/XX/XXXX**. SFTP (or SSH-based FTP) continues to be available through Forestry and we have no plans of removing support for this very viable deployment option.  
  
Existing sites that use FTP, FTP with Implicit SSL or FTP with TLS/SSL will be able to continue using it. However, new users and new sites won't be able to see this option anymore starting on the date mentioned above.  
  
We understand this might cause some issues for users that are new to the static space and that aren't familiar with other hosting options.   
  
To  those users I'd like to say: "This is where the good part starts!" You'll be able to deploy your new sites within seconds and likely save much of your annual costs by using the providers I outline below.

## How to deploy and host static sites in 2019

We put together a few tips and providers to make it easier for you to get started with static sites. The major selling point for these methods is that they distribute your site across multiple CDNs making your time to first byte ultra short. [We wrote about this before](https://forestry.io/blog/for-static-sites-theres-no-excuse-not-to-use-a-cdn/) and it was quite popular.

### Git-based deployment methods

In recent years providers such as Netlify, Github Pages or Zeit have caused quite a bit of a wave. These providers offer a very generous free plan, which is more than enough for most personal, non-profit or semi-commercial sites. 

Github Pages and Zeit simply take your repository and host it for you. This is more than enough and can easily be configured with Forestry. You'll use the deployment method "Github Pages" (limited to Github at the moment). We wrote a [quick guide](https://forestry.io/docs/hosting/github-pages/) on how to set up Github Pages (also applies to Zeit).

Netlify can also be used with Gitlab or Bitbucket and they offer some additional tooling. You can have them use a custom build command to built your site. To use Netlify with Forestry you simply need use the default deployment setting "Commit to source repo only".