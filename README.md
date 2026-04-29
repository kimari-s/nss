# nss

PHP + MySQL rewrite of the BBS scripts from あやしいわーるど＠上部構造 / ＠なごみ.
Active circa 2016–2023.

## Structure

```
sw.newsupers.net/
  index.php        Entry point / router
  Conf.php         Configuration
  Exec.php         Post / delete / like actions
  Node.php         Post model and HTML rendering
  View.php         Main view (threaded tree)
  View_min.php     Mobile view
  View_Tag*.php    Tag cloud / tag pages
  ViewSub_*.php    Partial views (links, new badge)
  Log.php          Access logging
  MyFeed.php       RSS 2.0 feed generator
  sub/UniFeedGen/  Feed writer library (third-party, GPL)
sql/
  nss.sql          Database schema
```

## Notes

- Sanitized for public archive — credentials and check logic removed
- This is not intended for production use

## Related

- [ks-strawberry-archive](https://github.com/kimari-s/ks-strawberry-archive) — Perl CGI predecessor (circa 2011–2017)
