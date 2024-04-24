---
title: Drafts Page
permalink: /drafts/
redirect_from:
  - /tag/draft
layout: page
---

Writing is cheap. Do more of it. This is one of my favorite drafts.

## "One Art" 3rd Draft

the art of losing isn’t hard to master:\
so many things seem almost to be meant\
to be lost, that their loss is no disaster.

Begin with car keys\
I’ll never\
the art of losing isn’t hrd to master

The practice brings losses, lose them faster,\
you’ll find your time well spent\
the mastered art of loss is no disaster.

<cite>Elizabeth Bishop.</cite>

## My drafts

{% for draft in site.drafts %}
  <li><a href="{{ draft.url }}">
      {{ draft.title }}
  </a></li>
{% endfor %}
