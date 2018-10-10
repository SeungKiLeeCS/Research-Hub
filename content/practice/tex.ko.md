---
title: "LaTex 렌더링"
date: 2018-10-10T10:51:17-05:00
draft: true
---

<!-- top of page -->
<!-- {{ if .GetParam "hasMath"}} -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.6.0/katex.min.css">
  <script src="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.6.0/katex.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.6.0/contrib/auto-render.min.js"></script>
<!-- {{ end }} -->


inline으로 sum을 표현하는 방법: `{{< tex "\sum_{n=1}^{\infty} 2^{-n} = 1" >}}` {{< tex "\sum_{n=1}^{\infty} 2^{-n} = 1" >}}.

Display Mode로 라텍스를 넣을 때는
    `{{< tex display="\int \frac{1}{x} dx = \ln |x|" >}}`
    {{< tex display="\int \frac{1}{x} dx = \ln |x|" >}}

<!-- bottom of page -->
<!-- {{ if .GetParam "hasMath"}} -->
  <script>renderMathInElement(document.body);</script>
<!-- {{ end }} -->