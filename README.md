# Minimal GraphQL v4 schema for Drupal

Reducing the [GraphQL Example](https://github.com/drupal-graphql/graphql/tree/8.x-4.x/examples/graphql_example)
module to a minimal implementation.

It only supports the following query.

```graphql
{
  article(id: 1) {
    id
    title
    author
  }
}
```

It is related to this [blog post](https://colorfield.be/blog/graphql-with-drupal-10-part-1-the-big-picture) and
used as a documentation to show that only 2 files
are needed to start a GraphQL 4 schema:
- graphql/minimal.graphqls
- src/Plugin/GraphQL/Schema/MinimalSchema.php
