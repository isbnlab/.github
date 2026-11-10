# ISBNLab

**Book metadata by ISBN, for developers.** [ISBNLab](https://www.isbnlab.com/) is a catalog of more than 100 million book editions, with a REST and GraphQL API for looking up books, authors, publishers, subjects and BISAC genres, and for validating and converting ISBN-10, ISBN-13, EAN and ASIN.

This organization holds the official ISBNLab API SDKs, generated from our [OpenAPI specification](https://www.isbnlab.com/api/docs.jsonopenapi), and open-source tools for working with ISBNs.

## Quick start

1. [Create a free account](https://www.isbnlab.com/register) and copy your API token.
2. Look up a book:

```bash
curl 'https://www.isbnlab.com/api/book/isbn/9780765302304' \
  -H 'accept: application/json' \
  -H 'Authorization: Bearer YOUR_API_TOKEN'
```

You get back the title, authors, publishers, series, genres, formats, page count, description and every other edition of the same book.

## The API

| Endpoint | What it returns | Plan |
|---|---|---|
| [Book data](https://www.isbnlab.com/api-information/api-book-data-documentation) | One edition by ISBN-10, ISBN-13 or ASIN | Free |
| [ISBN tools](https://www.isbnlab.com/api-information/api-isbn-tools-documentation) | Validate and convert ISBN-10, ISBN-13, EAN and ASIN | Free |
| [Book covers](https://www.isbnlab.com/api-information/api-book-cover-data-documentation) | Cover image URLs by ISBN or ASIN | Standard |
| [Authors](https://www.isbnlab.com/api-information/api-author-data-documentation), [publishers](https://www.isbnlab.com/api-information/api-publisher-data-documentation), [subjects](https://www.isbnlab.com/api-information/api-subject-data-documentation), [genres](https://www.isbnlab.com/api-information/api-genre-data-documentation) | Records by name, id, registrant prefix or BISAC code | Standard |
| [Book search](https://www.isbnlab.com/api-information/api-book-search-documentation) | Search by title, author or ISBN | Pro |
| [Other editions](https://www.isbnlab.com/api-information/api-book-related-editions-data-documentation) | Every edition of a book, plus the previous and next by date | Pro |
| [GraphQL](https://www.isbnlab.com/api/graphql/graphiql) | The same lookups as GraphQL queries | Pro |

The Free plan includes 1,000 calls a day. See [pricing](https://www.isbnlab.com/pricing) for Standard and Pro.

- [API documentation](https://www.isbnlab.com/api-information)
- [Interactive API reference](https://www.isbnlab.com/api/docs)
- [OpenAPI specification (JSON)](https://www.isbnlab.com/api/docs.jsonopenapi)

## Free ISBN tools on the web

- [ISBN search](https://www.isbnlab.com/isbn/tools/isbn-search)
- [ISBN-10 to ISBN-13](https://www.isbnlab.com/isbn/tools/isbn10-to-isbn13-converter) and [ISBN-13 to ISBN-10](https://www.isbnlab.com/isbn/tools/isbn13-to-isbn10-converter)
- [EAN to ISBN](https://www.isbnlab.com/isbn/tools/ean-to-isbn-converter) and [ISBN to EAN](https://www.isbnlab.com/isbn/tools/isbn-to-ean-converter)
- [ASIN to ISBN](https://www.isbnlab.com/isbn/tools/asin-to-isbn-converter) and [ISBN to ASIN](https://www.isbnlab.com/isbn/tools/isbn-to-asin-converter)
- [All tools](https://www.isbnlab.com/isbn/tools)

## Learn more

[Book database](https://www.isbnlab.com/book-database) · [How it works](https://www.isbnlab.com/how-it-works) · [FAQ](https://www.isbnlab.com/frequently-asked-questions) · [Blog](https://www.isbnlab.com/blog) · [Contact](https://www.isbnlab.com/contact-us)

Questions or SDK requests: open an issue in the relevant repository or email hello@isbnlab.com.
