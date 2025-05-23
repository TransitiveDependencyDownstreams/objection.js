---
home: true
heroText: Objection.js
tagline: An SQL-friendly ORM for Node.js
actionText: Get Started →
actionLink: /guide/installation
footer: MIT Licensed | Copyright © 2015-present Sami Koskimäki
---

Objection.js is an [ORM](https://en.wikipedia.org/wiki/Object-relational_mapping) for [Node.js](https://nodejs.org/) that aims to stay out of your way and make it as easy as possible to use the full power of SQL and the underlying database engine while still making the common stuff easy and enjoyable.

Even though ORM is the best commonly known acronym to describe objection, a more accurate description is to call it **a relational query builder**. You get all the benefits of an SQL query builder but also a powerful set of tools for working with relations.

Objection.js is built on an SQL query builder called [knex](https://knexjs.org). All databases supported by knex are supported by objection.js. **SQLite3**, **Postgres** and **MySQL** are [thoroughly tested](https://github.com/Vincit/objection.js/actions).

What objection.js gives you:

- **An easy declarative way of [defining models](/guide/models.html) and relationships between them**
- **Simple and fun way to [fetch, insert, update and delete](/guide/query-examples.html) objects using the full power of SQL**
- **Powerful mechanisms for [eager loading](/guide/query-examples.html#eager-loading), [inserting](/guide/query-examples.html#graph-inserts) and [upserting](/guide/query-examples.html#graph-upserts) object graphs**
- **Easy to use [transactions](/guide/transactions.html)**
- **Official [TypeScript](https://github.com/Vincit/objection.js/blob/main/typings/objection/index.d.ts) support**
- **Optional [JSON schema](/guide/validation.html) validation**
- **A way to [store complex documents](/guide/documents.html) as single rows**

What objection.js **doesn't** give you:

- **A custom query DSL. SQL is used as a query language.**
  This doesn't mean you have to write SQL strings though. A query builder based on [knex](https://knexjs.org) is
  used to build the SQL. However, if the query builder fails you for some reason, raw SQL strings can be easily
  written using the [raw](/api/objection/#raw) helper function.
- **Automatic database schema creation and migration from model definitions.**
  For simple things it is useful that the database schema is automatically generated from the model definitions,
  but usually just gets in your way when doing anything non-trivial. Objection.js leaves the schema related things
  to you. knex has a great [migration tool](https://knexjs.org/guide/migrations.html) that we recommend for this job. Check
  out the [example project](https://github.com/Vincit/objection.js/tree/main/examples/koa-ts).

The best way to get started is to clone our [example project](https://github.com/Vincit/objection.js/tree/main/examples/koa) and start playing with it. There's also a [typescript version](https://github.com/Vincit/objection.js/tree/main/examples/koa-ts) available.

Check out [this issue](https://github.com/Vincit/objection.js/issues/1069) to see who is using objection and what they think about it.
