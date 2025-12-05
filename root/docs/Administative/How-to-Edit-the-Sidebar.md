# How to Edit the Sidebar

Wiki has a lot of limitations, including no easy support for subpages. Essentially every page in the repository is stored in only one singular folder, there are no subpages of anything. The folders you might see if you pulled the repository are purely for organizational purposes and do not contribute to the structure of the sidebar

The sidebar is all typed out manually. It is not enjoyable to do, but it's what works with the limited capabilities of GitHub Wiki

The general structure should be:

- Home
- Subsection as a dropdown list
- More subsections as dropdown list

In order to make dropdown lists in Markdown you have to use HTML tags. The details tag is what makes the dropdown list while summary tag gives it the title. If you have never used HTML before, essentially you just define elements using `<element_name>` and then define the things inside it, and when you're done you close it with the same element name but prepended with a /, so `</element_name>`

Inside these HTML tags there will be bullet points with hyperlinks to the specific pages, so you'd do

```HTML
<details>
<summary>Subsection name</summary>

- Page bullet points go here as hyperlinks
- To make a hyperlink all you have to do is [whatever you want the display name to be](link)

</details>
```

Whenever a new page is added to the wiki it should be added to the sidebar

> Author: Ella Moody (https://github.com/TheThingKnownAsKit)