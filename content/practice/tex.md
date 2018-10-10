---
title: "LaTex"
date: 2018-10-10T10:51:17-05:00
draft: true
---

<!-- top of page -->
{{ if .GetParam "hasMath"}}
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.6.0/katex.min.css">
  <script src="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.6.0/katex.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.6.0/contrib/auto-render.min.js"></script>
{{ end }}


Here's sum inline math: {{< tex "\sum_{n=1}^{\infty} 2^{-n} = 1" >}}.

Display mode math looks like
    {{< tex display="\int \frac{1}{x} dx = \ln |x|" >}}

<!-- bottom of page -->
{{ if .GetParam "hasMath"}}
  <script>renderMathInElement(document.body);</script>
{{ end }}