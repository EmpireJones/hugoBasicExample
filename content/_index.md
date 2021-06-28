+++
author = "Hugo Authors"
+++

When running <code>hugo server</code> (i.e. live reload without a full build), if you modify some files, such as index.html (layout) or fancy-header.html (partial on the page) the page's scratch gets cleared, but side effects from shortcodes don't get re-processed, causing the todo summary section of the page to not show until the next full build.


## Todo List with Details

{{< addTodo >}}
# Do thing one
{{</ addTodo >}}

Here's some more info about thing 1...


{{< addTodo >}}
# Do thing two
{{</ addTodo >}}

Here's some more info about thing 2...