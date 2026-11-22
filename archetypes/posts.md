---
title: "{{ replace .Name "-" " " | title }}"
date: {{ now.Format "2006-01-02" }}
language: en
description: ""
hook: ""
hero_image: ""
hero_alt: ""
hero_caption: ""
player_quote: ""
---

{{< toc >}}
<ol>
  <li><a href="#section-one">Section one</a></li>
</ol>
{{< /toc >}}

## Section One

{{< takeaways >}}
**Key takeaway one.**

**Key takeaway two.**
{{< /takeaways >}}

{{< figure src="/images/example.jpg" alt="Describe the image" caption="A caption for the figure." >}}

Body text goes here.

{{< players >}}"A memorable line from the table." — players{{< /players >}}

{{< aside >}}A right-aligned margin note.{{< /aside >}}
