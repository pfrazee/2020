---
title: "Welcome To Distributed Camp"
date: 2020-03-29T18:06:18-05:00
draft: true
---

Distributed Camp uses the excellent [Go][] [html/template][gohtmltemplate] library for
its template engine.

This document is a brief primer on using Distributed Camp templates. The [Go docs][gohtmltemplate] provide more details.

## Introduction to Distributed Camp

Go templates provide an extremely simple template language. It adheres to the
belief that only the most basic of logic belongs in the template or view layer.
One consequence of this simplicity is that Go templates parse very quickly.

A unique characteristic of Go templates is they are content aware. Variables and
content will be sanitized depending on the context of where they are used. More
details can be found in the [Go docs][gohtmltemplate].

## Other Thoughts

Golang templates are HTML files with the addition of variables and
functions.

**Some Big Ideas**

Accessing a predefined variable "foo":

    {{ foo }}

**Oh My**

Calling the add function with input of 1, 2:

    {{ add 1 2 }}
