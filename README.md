# Quote Editor on Rails 8.1 with esbuild

Inspired by https://www.hotrails.dev/turbo-rails/crud-controller-ruby-on-rails

```bash
rails new quote-editor --css=sass --javascript=esbuild --database=postgresql
```

```bash
mkdir ../quote-editor-db
initdb-17 -D ../quote-editor-db
pg_ctl-17 -D ../quote-editor-db --log=log/devdb.log -o "-p 5436" start
pg_ctl-17 -D ../quote-editor-db stop
```

## Running specs

```bash
bin/rails test:system
```
