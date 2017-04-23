---
layout: post
title: 'Recipe:  Thread safe queue'
date:   2017-04-22 01:06:05 +0200
categories: cpp
---

The C++11 queue implementation is not thread safe... It is a common requeriment to have a concurrent access in a C++ queue, the most simple option is the implementation of a
decorator pattern and it adds two new operations to synchronize the access

<script src="https://gist.github.com/carlosb1/8b806b9b9bb2a6914ee7.js"></script>
