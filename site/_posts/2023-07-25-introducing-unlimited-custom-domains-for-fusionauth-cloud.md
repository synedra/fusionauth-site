---
layout: blog-post
title: Introducing Unlimited Custom Domains for FusionAuth Cloud
description: FusionAuth announces Unlimited Custom Domains for FusionAuth Cloud, allowing you to associate another domain with your FusionAuth Cloud deployment without having to fuss with certificate issuance and renewal
author: Emily Jansen
image: blogs/unlimited-custom-domains/unlimited-custom-domains.png
category: announcement
tags: topic-press-release fusionauth company cloud press-release
excerpt_separator: "<!--more-->"
---

Today, we’re announcing Unlimited Custom Domains for [FusionAuth Cloud](https://fusionauth.io/platform/fusionauth-cloud). Custom domains allow you to associate another domain with your FusionAuth Cloud deployment without having to fuss with certificate issuance and renewal – it just works.

<!--more-->

Let’s take a look at the changes now and stay tuned for a future blog on how we engineered this feature (hint - it involves [Caddy](https://caddyserver.com/), an open-source project we are proud to support).

## What are Custom Domains?

Custom domains let you brand your login experience and have your users see a domain they recognize – yours. Instead of seeing `piedpiper.fusionauth.io ` in your login page’s URL, adding a custom domain allows you to set it as `auth.piedpiper.com. `


## But Wait, Custom Domains Aren’t New

That’s true! Custom domains have been available for FusionAuth Cloud since 2021, but we supported a maximum of 4 custom domains, even on our High Availability hosting plan. Adding more than that required using a [proxy](https://fusionauth.io/docs/v1/tech/admin-guide/proxy-setup) layer like CloudFlare, Apache, or CloudFront and extra work for FusionAuth Cloud customers to manage those domains and certificates.

That got us thinking… why limit it to 4? And how could we streamline the process for customers?

**So as of today, these changes are now in effect for FusionAuth Cloud:**

* High Availability Hosting now can optionally include Unlimited Custom Domains.  Please ask your support and sales teams for more information about what is required to turn this on.
* A streamlined user interface for managing custom domains within the FusionAuth admin portal.

{% include _image.liquid src="/assets/img/blogs/unlimited-custom-domains/fusionauth-cloud-custom-domains.png" alt="Introducing Unlimited Custom Domains." class="img-fluid" figure=false %}

## How to Add a Custom Domain

If you are on a supported deployment and want a custom domain name such as `auth.piediper.com`, it’s now entirely self-service. Log in to your account portal, navigate to **Deployments** and then select **Custom URL(s)** under the **Action** dropdown. Check out the custom domains [documentation](/docs/v1/tech/installation-guide/cloud#unlimited-custom-domains) for details about how to add the domain name and update an existing domain record.

{% include _image.liquid src="/assets/img/blogs/unlimited-custom-domains/managing-domains-fusionauth-cloud.png" alt="Managing a Custom Domain." class="img-fluid" figure=false %}

Other customer identity and access management platforms typically only offer one custom domain as standard. If you need more than that, some vendors even make you pay an extra fee per domain. With FusionAuth, it’s just another feature we are adding to support our [growing customer base](/blog/2023/03/15/winning-customer-auth-market).

FusionAuth Cloud offers different hosting tier selections to give you a choice for your deployment needs. All plans include a private instance (no shared public cloud) fully managed by FusionAuth, with options for backup, custom availability zones, uptime SLAs, and more to meet your infrastructure requirements.

You can start a [free trial of FusionAuth Cloud](https://fusionauth.io/pricing?step=hosting) now or for more complex projects or infrastructure questions, reach out to our [identity experts](https://fusionauth.io/contact) for help.