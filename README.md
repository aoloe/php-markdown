# php-markdown

wrapper around Michelf's markdown class

- adds support or paragraph classes and ids:

        {.class .id}
        the paragraph

- adds a filter for urls of local links and imagesges
- convert ' -- ' through `&ndash;` (other typographic features planned)
- converts markdown inside of `<td>` elements

## Inspiration that could come from Scholarly-Markdown

<http://scholarlymarkdown.com/Scholarly-Markdown-Guide.html>

- `##this is a title {#anchor-to-it}`  
  `this is a normal paragraph {#anchor-to-it}`  
  the anchor is at the end of the line, with no space between the # and the end of line  
  `##this is a title #anchor-to-it`  
  `this is a normal paragraph #anchor-to-it`
- scholarly-md defines  
      \`\`\`math_def {latex math definitions}\`\`\`  
  we could use it for the external filter definition, too  
      \`\`\`csv:....\`\`\`
- metadata: a multiline pre-formatted block at the beginning or at the end of the file, with the fields defined as YAML.  
          ~~~
          author: Me Myself
          ~~~

## notes

- [vfmd](http://www.vfmd.org/vfmd-spec/syntax/) is a variant of Markdown with an unambiguous specification of its syntax.
- [Bootstrap-Markdown](http://www.codingdrama.com/bootstrap-markdown/) designed to be easily integrated with your bootstrap project. It exposes useful API that allow you to fully hook-in into the plugin
