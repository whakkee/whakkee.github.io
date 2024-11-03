---
draft: true
author: Hugo Authors
title: Math Typesetting
date: 2019-03-08
description: A brief guide to setup KaTeX
---

Mathematical formulas written in LaTeX notation can be rendered to HTML without using javascript.<!--more-->
Rendering can take place either globally, or in specific locations using a built-in shortcode.

1. To render math globally, [enable the passthrough extension](https://gohugo.io/content-management/mathematics/) in the site configuration.

    ```
    Inline formulas such as $y=ax+b$ are supported, displayed formulas as well:

    $$
      e^{i\pi}+1=0
    $$
    ```

2. To render mathematical expressions in specific locations, surround them with the `math` shortcode:

    ```
    Inline formulas such as {{</* math */>}}y=ax+b{{</* /math */>}} are supported, displayed formulas as well:

    {{</* math displayMode=true */>}}
      e^{i\pi}+1=0
    {{</* /math */>}}
    ```

**Note:** Use the online reference of [Supported TeX Functions](https://katex.org/docs/supported.html)

### Examples

Inline math: $$\varphi = \dfrac{1+\sqrt5}{2}= 1.6180339887…$$

Block math:
$$
 \varphi = 1+\frac{1} {1+\frac{1} {1+\frac{1} {1+\cdots} } } 
$$
