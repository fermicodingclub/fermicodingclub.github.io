---
layout: post
title: "Specifications for an ACNET web app"
date: 2019-01-06 20:12:40 -0600
categories: ACNET web JavaScript CSS HTML
---

# ACNET Parameter Page

The parameter page application is the multi-tool of Fermilab accelerator operators. ACNET parameters are an abstraction of the features that you expect when interacting with hardware in the field. Generally, these properties include reading, setting, status, and control. The parameter page not only gives operators access to each and all of these properties but unlocks a super-power when a selection of related parameters are on the same page.

To begin this project, we should identify the core features of the parameter page that makes it function. Many features have been combined over the years to create what we know as the parameter page now. By limiting the number of features to a functional set, we can prevent this project from becoming overwhelming.

## List of features

The first thing we can observe is that we are presented with essential information for the parameters on the page.

- Display basic device properties
  - Setting boolean
  - Parameter name
  - Parameter description
  - Current Setting D/A
  - Alarm bypass boolean
  - Current Reading A/D
  - Parameter units
  - Current status

![parameter page with descriptions](/assets/images/param-page.png)

Several of the features of this application are not immediately visible to the user like the boolean settings and alarm bypass bits. The operator must know that these features exist for their absence to have meaning. Hidden features are something we should consider in the future when discussing how to improve the application. For now, let's keep it simple and focus on replicating what exists.

Other features that are not visible without user interaction include:

- Addition of parameters to the page
- Removal of parameters to the page
- Previous setting
  - Return to the previous setting
- Setting control
  - Setting multiplier
- Digital control
- Setting multiple parameters with one "knob"

Other features are not parameter related also:

- Comments
- Math
- Save current page for persistence

## Essential features

Broadly the purpose of this application is to display the properties of parameters on a given page. We can keep our implementation simple by restricting our first pass to reading and displaying the visible properties I outlined above. We have done most of the work for this in a [previous Coding Club meeting about web development](https://github.com/beauremus/codingclub/blob/master/presentations/webDevelopment/webDevelopment.pdf). I demoed [WebDPM](https://cdcvs.fnal.gov/redmine/projects/acsys-dpm/wiki/WebDPM_Apps) that allowed us to have live readings of a parameter in the browser.

## Choosing tools

I have already specified that we will use the browser, but beyond that, we are free to use whatever tools individually solve our problems. For many, including myself, it can be easy to spend all your time learning and evaluating tooling. Let us set out to use default browser features as much as possible and only introduce tools when we need a new feature, or it makes our job easier.

There are tropes about JavaScript that turn people away. These tropes present a sense of instability that JavaScript is unstable and constantly changing. There is a sense that there are no standards because as soon as the next tool comes out, we will all shift to that tool. While this may have been true in the past (not really), the truth is that monoliths like Mozilla, Google, Microsoft, and Apple all have a stake in making the web a stable platform. They all have browsers that they want to be performant and compliant; otherwise, developers and users alike will not use them. All of these organization participate standards organizations like [W3C](https://www.w3.org/) and [ECMA](https://www.ecma-international.org/). They are then the ones who implement the standards. For better or worse this is the development pipeline for the web now. [WHATWG](https://whatwg.org/) is an open spec that is also influential.

All of that to say, the web is a great place to be a developer.
