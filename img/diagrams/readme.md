# Diagrams-as-Code

There are two methods to create diagrams-as-code that can be  viewed and managed in Github. Both methods require use of Visual Studio Code (VSCode) and specific VSCode plugins.

### Graphical-based drawing
* In VSCode create Draw.io file (*.drawio)
* Edit in VSCode using the Draw.io plugin. 
  * Optional:
  * insert custom icons via icon plugins (AWS, etc)
  * insert Mermaid text diagram 
  * add white bounding box around entire figure
* Save as .drawio
* Export as .svg (not PNG - it is pixellated)
* Preview SVG in VSCode

### Text-based drawing
* In VSCode create Markdown file (*.md)
* Add and edit Mermaid syntax in ```mermaid section. 
  * Optional:
  * insert AI-generated Mermaid code (Claude, ChatGPT)
  * insert Mermaid code from examples and templates 
* Embed/link SVG, PNG diagrams 
  * link SVG diagrams (created in Draw.io above}
  * link PNG diagrams (from any other source}
  * embed raw SVG code
* Save as .md
* Preview in VSCode (need Markdown and Mermaid plugins)


__VSCode Plugins__
* [mermaid preview](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-mermaid)  
* [mermaid syntax highlighting](https://marketplace.visualstudio.com/items?itemName=bpruitt-goddard.mermaid-markdown-syntax-highlighting)  
* [draw.io plugin for mermaid](https://marketplace.visualstudio.com/items?itemName=nopeslide.vscode-drawio-plugin-mermaid)  
* [SVG edit and preview](https://marketplace.visualstudio.com/items?itemName=jock.svg)




## Reference
__Mermaid__
* [mermaid getting started](https://mermaid.js.org/intro/getting-started.htm)
* [mermaid syntax](https://mermaid.js.org/intro/syntax-reference.html)
* [diagrams as code in github](https://www.freecodecamp.org/news/diagrams-as-code-with-mermaid-github-and-vs-code)  

__Draw.io__  
* [insert shapes, links, templates and more in drawio diagram](https://www.drawio.com/doc/faq/arrange-insert-menu)
* [embed Markdown in drawio diagram](https://www.drawio.com/blog/embed-diagrams-github-markdown)
* [embed Mermaid in drawio diagram](https://www.drawio.com/blog/mermaid-diagrams)
* [export drawio diagram as svg](https://www.drawio.com/doc/faq/export-to-svg)  
