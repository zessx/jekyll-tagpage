# jekyll-tagpage
Jekyll tag page generator

## Installation
Just copy both `_layouts` and `_plugins` folder into your Jekyll project.

## Usage
Add tags to your posts using the `tags` predefined variable:

    ---
    layout: post
    title:  "Lorem ipsum post"
    date:   2015-05-18
    tags:
    - foo
    - bar
    --- 

You can also use a compressed version:

    ---
    layout: post
    title:  "Lorem ipsum post"
    date:   2015-05-18
    tags: [foo, bar, baz]
    --- 

The plugin will generate this structure:

    _site/
      lorem-ipsum-post/
      tag/
        foo/
        bar/

## Customization
jekyll-tagpage comes with 3 options, that you can override in your `_config.yml` file:

- `tag_dir`: tag pages' directory (default: `tag`)
- `tag_title_prefix`: prefix for the tag page's title (default: empty)
- `tag_title_suffix`: suffix for the tag page's title (default: empty)
