# php-markdown

wrapper around Michelf's markdown class

- adds support or paragraph classes and ids:

        {.class .id}
        the paragraph

- adds a filter for urls of local links and imagesges
- convert ' -- ' through `&ndash;` (other typographic features planned)
- converts markdown inside of `<td>` elements
