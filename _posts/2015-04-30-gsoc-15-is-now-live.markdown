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

Enhance the performance of the asset compilation process of Ruby on Rails. At first, some benchmarks
of the current state of some well-known rails-based projects will be needed. Then contrast different
alternatives to the current options, maybe integrate them too. If the results are not satisfactory,
propose substitutes and even implementing them.

## Evented File System Monitoring

**Student:** [Puneet Agarwal](https://github.com/puneet24)    
**Mentors:** [Xavier Noria](https://github.com/puneet24) and [Matthew Draper](https://github.com/matthewd)

Ruby On Rails consists of a very powerful API called the File Checker API which serves the epic
feature of dynamic reloading. This project deals with improving the current implementation as a
substitute. The final output of the project will be an alternative to the existing File Checker that
is, the Evented File System Monitoring gem which will be best optimized for the Rails framework.

## Asset Pipeline Support for Source Maps

**Student:** [Andrei Istratii](https://github.com/Andreis13)    
**Mentors:** [Arthur Nogueira Neves](https://github.com/arthurnn) and [Rafael Mendonça França](https://github.com/rafaelfranca)

The project is supposed to add support for Javascript and CSS source-maps generation functionality
to the Rails Asset Pipeline. This has a potential of making it easier to debug and inspect client
code in production environments as well as situations when the assets are minified or are compiled
from another language like Coffeescript.

## Refactoring ActiveSupport and ActionView

**Student:** [Islam Wazery](https://github.com/wazery)    
**Mentors:** [Kir Shatrov](https://github.com/kirs) and [Carlos Antonio da Silva](https://github.com/carlosantoniodasilva)

This project is a refactoring project for Rails, it consists of some refactoring work like
refactoring ActiveSupport::Parameters to not depend on Ruby's standard Hash also
ActionView::OutputBuffer needs to not depend on Ruby's standard String (through
ActiveSupport::SafeBuffer. ActionView helpers can provide a new API using the new Ruby 2 first class
support for keyword arguments, building on the ground work of Kirill on merged PR#18323. Also
ActionView needs to be decoupled from ActionPack.

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
