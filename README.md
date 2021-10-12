# Heroku Buildpack for Custom Fonts

Fonts used by [Practio](https://www.practio.com) for printing documents.

This buildpack is very specific to our needs. It can and will change and **YOUR APP WILL BREAK**.
Even the fonts in `fonts.tar.gz` are _probably not what you want or expect_.

We'd hate to see that happen. But please feel free to fork it or crib ideas to make it your own, though!

## Development

### How to Update Fonts Archive

Move individual TTF (only TTF) files into `fonts`

```
tar -czvf fonts.tar.gz fonts
```

### Original Inspiration

- https://github.com/CoffeeAndCode/puppeteer-heroku-buildpack
- https://github.com/debitoor/heroku-buildpack-converter-fonts
