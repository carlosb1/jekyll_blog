---
layout: post
title: Double checked problem for concurrency
categories: cpp
---

This weekend, I read an article from Uncle Bob to optimise the access to thread-safe objects [link](https://app.box.com/s/t7kvebv4p8yiu5jfrr69ldujs7rqzdlw)

The problem is explained with a Singleton pattern implemention (without smart pointers):

<script src="https://gist.github.com/carlosb1/98008c218aa3ec367d563e2932136b3c.js"></script>

The problem how to evaluate the critical section efficiently. For this, it is necessary take care our blocking threads are trying to access to the critical session
in a different time and 'software state' where in this state is possible has initialized our critical resource. The solution is:

<script src="https://gist.github.com/carlosb1/1ecb788fa7bfae316c2cbd7f4054e64c.js"></script>


