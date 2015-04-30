---
layout: post
title: Google Summer of Code 2015 is now live!
categories:
- activism
author: febuiles
published: true
date: 2015-04-28 15:00:00 +00:00
---

**TODO**: Replace project descriptions with something readable.
**TODO**: Add line thanking sponsors.
**TODO**: Change published flag and set date/time when ready.

Google has announced the list of [accepted projects][melange] for this year's [Google Summer of
Code][gsoc] (GSoC). Rails has been granted 8 slots, here's a brief introduction to the projects and
the people behind them.

## Performance Enhancements for the Asset Pipeline

**Student:** [Martha de Luque]()    
**Mentors:** [Guillermo Iguaran](https://github.com/guilleiguaran) and [Joshua Peek](https://github.com/josh)

Martha will be profiling, benchmarking and updating parts of our asset compilation process to
improve our asset [re]generation speed. The initial scope of this project covers CoffeeScript, Sass and
Uglifier, but benchmarks will be guiding this effort to work where we can get the biggest benefits.

## Evented File System Monitoring

**Student:** [Puneet Agarwal](https://github.com/puneet24)    
**Mentors:** [Xavier Noria](https://github.com/puneet24) and [Matthew Draper](https://github.com/matthewd)

Our File Checker API is due for a makeover. It has served us well over the years, we're done with
polling. Puneet will be replacing our current design with a event-based approach that relies
on existing third-party monitors (e.g. `inotify` or `FSEvent`).

## Asset Pipeline Support for Source Maps

**Student:** [Andrei Istratii](https://github.com/Andreis13)    
**Mentors:** [Arthur Nogueira Neves](https://github.com/arthurnn) and [Rafael Mendonça França](https://github.com/rafaelfranca)

The goal of Andrei's project is to give you good inspecting and debugging capabilities in environments
where your code goes through various transformations (e.g. your CoffeeScript file being compiled to
Javascript and then minified in your staging environment). With source maps you can use the existing
tools your browser provides to do things like reading the CoffeeScript source or setting breakpoints
on it.

## Refactoring ActiveSupport and ActionView

**Student:** [Islam Wazery](https://github.com/wazery)    
**Mentors:** [Kir Shatrov](https://github.com/kirs) and [Carlos Antonio da Silva](https://github.com/carlosantoniodasilva)

Islam is adding some of the stuff we love to see in Rails, liked named arguments
 for ActionView helpers (goodbye counting commas!) or removing the ActiveSupport dependency on
 ActionPack. He will also be investigating how to improve some of our core abstractions like
 [ActionController::Parameters](http://edgeapi.rubyonrails.org/classes/ActionController/Parameters.html)
 and [ActionView::OutputBuffer](http://tenderlovemaking.com/2014/06/04/yagni-methods-slow-us-down.html).

## Web Console Browser Extensions

**Student:** [Hiroyuki Sano](https://github.com/sh19910711)    
**Mentor**: [Genadi Samokovarov](https://github.com/gsamokovarov)

The web-console is a debugging tool for Ruby on Rails web applications. It provides an interactive Ruby session to debug in the web browser. The session in the console has the context of the code of the web application. The goal of this project is to create the browser extensions of web-console. It allows to display the console aside from the web application's view. By doing this, the console can be displayed without breaking affects to the view code of the web application.

## Test Failure Prediction

**Student:** [Genki Sugimoto](https://github.com/Genki-S)    
**Mentors:** [Robin Dupret](https://github.com/robin850), **TODO** Confirm: "and maybe Josh K from travis CI"

Take Aaron's ideas (http://tenderlovemaking.com/2015/02/13/predicting-test-failues.html) a bit further.

## Refactoring Cookies

**Student:** [Siddharth Bhatore](https://github.com/sbhatore)    
**Mentors:** [Kasper Timm Hansen](https://github.com/kaspth) and [Prem Sichanugrist](https://github.com/sikachu)

Refactor Rails' Cookie Implementation and Improve Signing with Expiry and Purpose
Current Rails Cookie System does not have a mechanism to expire a cookie, and purpose of a cookie is
not defined. Apparently, cookies are not very secure. This project will make the expiry of cookies
possible on the server side and also add purpose field for cookies. To make this integration with
the current structure, I will also refactor the cookie internals. Upgrade paths will also be taken
care of, so that cookies are readable even after a user upgrades his application.

## Improving RubyBench.org

**Student:** [Kasif Gilbert](https://github.com/klgilbert)    
**Mentors:** [Sam Saffron](https://github.com/SamSaffron)

continuous benchmarking for Rails, JRuby support, fixing failures current failures, http://rubybench.org/rails/rails/releases

* * *

**Fun Fact**: 5 of the 13 mentors we have this year participated as GSoC students in previous years. Today they're all
  core members or active contributors. **TODO** Confirm math, update if Josh K. is added.

And in case you missed it, Ruby and SciRuby will also be part of this year's GSoC. You can learn
more in the [Ruby GSoC][rubygsoc-ml] and [SciRuby
Development][sciruby-ml] mailing list announcements.


[gsoc]: https://www.google-melange.com/gsoc/homepage/google/gsoc2015
[melange]: http://www.google-melange.com/gsoc/projects/list/google/gsoc2015
[rubygsoc-ml]: https://groups.google.com/forum/?hl=en#!topic/rubygsoc/u_BabU5Nmvo
[sciruby-ml]: https://groups.google.com/forum/?hl=en#!topic/sciruby-dev/ijd2KOh9WNc
