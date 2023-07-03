---
title: "Post 1"
publishDate: "1 Jan 2006"
---

{{< html >}}
<ul>
{{ range .Pages.ByPublishDate }}
<li>
<h1><a href="{{ .Permalink }}">{{ .Title }}</a></h1>
<time>{{ .Date.Format "2 Jan 2006" }}</time>
</li>
{{ end }}
</ul>
{{< /html >}}