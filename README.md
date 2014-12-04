# Jekyll::API

Create APIs from Jekyll page data.

## Installation

Follow [Jekyll's instructions for installing Jekyll plugins](http://jekyllrb.com/docs/plugins/#installing-a-plugin). The **Jekyll::API** plugin is available from the `jekyll-api` gem.

## Usage

1. Define data as front-matter in your Markdown Jekyll pages.
2. Enjoy the API.

For example, the **Jekyll::API** plugin will generate a `/people/jill/data.json` file

```json
{
  "name": "Jill"
}
```

 using the Jekyll page `/people/jill.md`.
```yaml
---
name: Jill
---
Hi, my name is {{ page.name }}
```

If you set `permalink: pretty` in your `_config.yml`, the resulting HTTP endpoints will be:
* HTML - `/people/jill/`
* JSON - `/people/jill/data.json`

## Contributing

1. Fork it (https://github.com/gregoryjscott/jekyll-api/fork).
2. Create your feature branch (`git checkout -b my-new-feature`).
3. Commit your changes (`git commit -am 'Add some feature'`).
4. Push to the branch (`git push origin my-new-feature`).
5. Create a new Pull Request.
