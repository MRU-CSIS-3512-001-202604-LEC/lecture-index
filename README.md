# Lecture Demo Index - COMP3512-001

**Fall 2026**

![Written by Claude (AI)](https://img.shields.io/badge/written%20by-Claude%20(AI)-D97757?style=for-the-badge)

_This index was written by Claude, an AI assistant made by Anthropic, from the code in each lecture repo._

Trying to remember where you saw something demonstrated? Look it up in the [topic lookup](#topic-lookup), then go to that lecture's section for the routes and files.

---

## Where the code is

Each lecture's demo code is in **your own copy** of that lecture's repo, the one you accepted through Classroom 50. Its name ends with the lecture and your GitHub username, like `...-lec-09-php-lec-08-yourusername`.

Three lectures were live-coded, so the finished code is in a public repo instead:

- Lec-02: [lec-02-php-lec-01-end](https://github.com/MRU-CSIS-3512-001-202604-LEC/lec-02-php-lec-01-end)
- Lec-03: [lec-03-php-lec-02-end](https://github.com/MRU-CSIS-3512-001-202604-LEC/lec-03-php-lec-02-end)
- Lec-07: [lec-07-php-lec-06-end](https://github.com/MRU-CSIS-3512-001-202604-LEC/lec-07-php-lec-06-end)

### Running a lecture repo

From the repo's folder:

```
php database/build.php
php -S localhost:8000 -t www/public www/public/index.php
```

Then open http://localhost:8000 and visit the routes listed below. You only need `build.php` for lectures that use the database (Lec-07 onward), and running it again resets the data. From Lec-11 on, the home page links to every demo.

In the JS lectures, the demo files are in `www/public/js/`. Each one is split into numbered STEPs: uncomment one step at a time and watch the console.

---

## Topic lookup

| Topic | Lecture | Where to look |
| --- | --- | --- |
| 404 page | [Lec-02](#lec-02---php-lec-01) | `www/views/404.php` |
| Aggregates: `COUNT`, `SUM`, `GROUP BY` | [Lec-08](#lec-08---php-lec-07), [Lec-10](#lec-10---php-lec-09) | `database/lecture/` SQL files; `drink_sales_starter()` |
| Alternative syntax (`if:` / `endif;`, `foreach:` / `endforeach;`) | [Lec-05](#lec-05---php-lec-04), [Lec-06](#lec-06---php-lec-05) | `/lab-schedule`; `/games-alt-syntax` vs `/games-std-syntax` |
| Array methods: `map`, `filter`, `find` | [Lec-16](#lec-16---js-lec-02), [Lec-17](#lec-17---js-lec-03) | Lec-16 `demo-04.js`; Lec-17 `demo-03.js` |
| Arrays (JS), `length`, `for...of` | [Lec-16](#lec-16---js-lec-02) | `demo-02.js` |
| Arrow functions | [Lec-16](#lec-16---js-lec-02) | `demo-01.js` |
| Authentication (logging in and out) | [Auth demo](#authentication-and-authorization-self-study) | `demo-02` |
| Authorization and roles | [Auth demo](#authentication-and-authorization-self-study) | `demo-02`, `demo-03` |
| Bound parameters (named placeholders like `:search`) | [Lec-09](#lec-09---php-lec-08), [Lec-10](#lec-10---php-lec-09) | `/demo/safe`, `/demo/safe-better`; `/drinks` |
| Callbacks, `forEach` | [Lec-16](#lec-16---js-lec-02) | `demo-03.js` |
| `COUNT(*)` vs `COUNT(column)` | [Lec-08](#lec-08---php-lec-07) | `lec-08-analytics-finished.sql`, Q2 |
| Controllers vs views | [Lec-02](#lec-02---php-lec-01) | `www/controllers/app/index.php`, `www/views/app/index.php` |
| Cookies: set, read, delete, path | [Lec-11](#lec-11---php-lec-10) | `/demo-01/...` |
| Cookies can't be trusted | [Lec-11](#lec-11---php-lec-10) | `/demo-02/join`, `/demo-02/discount` |
| `DatabaseQueries` class, `run()` and `fetchAll()` | [Lec-07](#lec-07---php-lec-06), [Lec-09](#lec-09---php-lec-08) | `www/queries/DatabaseQueries.php` |
| Dates and times (`DateTimeImmutable`) | [Lec-05](#lec-05---php-lec-04), [Lec-11](#lec-11---php-lec-10) | `/lab-schedule`; `/demo-03/time` |
| Debugging with `d()` and `dd()` | [Lec-07](#lec-07---php-lec-06), [Lec-10](#lec-10---php-lec-09) | `www/controllers/games.php`; `drinks.php` |
| DOM: create, append, remove elements | [Lec-18](#lec-18---js-lec-04) | `demo-02.js` |
| DOM: `querySelector`, `querySelectorAll` | [Lec-18](#lec-18---js-lec-04) | `demo-01.js` |
| DOM: render a list from data | [Lec-18](#lec-18---js-lec-04), [Lec-19](#lec-19---js-lec-05) | Lec-18 `demo-03.js`; Lec-19 `demo-04.js` |
| Events: `addEventListener` and the event object | [Lec-19](#lec-19---js-lec-05) | `demo-01.js` |
| Escaping output with `e()` | [Lec-02](#lec-02---php-lec-01), [Lec-04](#lec-04---php-lec-03), [Lec-09](#lec-09---php-lec-08) | home page; `/team`; `/demo/xss` |
| Flash messages | [Lec-12](#lec-12---php-lec-11), [Auth demo](#authentication-and-authorization-self-study) | `/demo-05/form`; login page |
| Form fields in JS: `value`, `checked`, radio buttons | [Lec-19](#lec-19---js-lec-05) | `demo-03.js` |
| Form validation on the server | [Lec-12](#lec-12---php-lec-11) | `/demo-02/form`, `www/helpers/order.php` |
| Forms: GET vs POST, `$_GET` and `$_POST` | [Lec-12](#lec-12---php-lec-11) | `/demo-01/form` |
| Functions are values (declarations, expressions) | [Lec-16](#lec-16---js-lec-02) | `demo-01.js` |
| "Headers already sent" | [Lec-11](#lec-11---php-lec-10) | `/demo-01/early` |
| `innerHTML` vs `textContent` | [Lec-18](#lec-18---js-lec-04) | `demo-04.js` |
| `input` event | [Lec-19](#lec-19---js-lec-05) | `demo-04.js` |
| Interpolation: `"$name"` and `"{$name}"` | [Lec-05](#lec-05---php-lec-04) | `/interpolation` |
| JSON | [Lec-17](#lec-17---js-lec-03) | `demo-03.js` |
| `LEFT JOIN` and `COALESCE` | [Lec-08](#lec-08---php-lec-07), [Lec-10](#lec-10---php-lec-09) | `database/lecture/` SQL files; `drink_sales_starter()` |
| Links built in the controller (`http_build_query()`) | [Lec-10](#lec-10---php-lec-09) | `www/controllers/drinks.php` |
| Modules: `import` and `export` | [Lec-17](#lec-17---js-lec-03) | `demo-05.js`, `demo-05-helpers.js` |
| `Number()`, `NaN` and the `+` trap | [Lec-15](#lec-15---js-lec-01) | `demo-03.js` |
| Null coalescing (`??`) | [Lec-03](#lec-03---php-lec-02), [Lec-10](#lec-10---php-lec-09) | `www/controllers/msg/index.php`; `drinks.php` |
| Objects (JS): dot and bracket access | [Lec-17](#lec-17---js-lec-03) | `demo-01.js` |
| Objects are shared, not copied | [Lec-17](#lec-17---js-lec-03) | `demo-02.js` |
| Partials | [Lec-04](#lec-04---php-lec-03), [Lec-06](#lec-06---php-lec-05) | `/callout-demo`, `/team`; `/games-alt-with-partials` |
| Password hashing | [Auth demo](#authentication-and-authorization-self-study) | `demo-01` |
| Path parameters (`/nmsg/:colour`) | [Lec-03](#lec-03---php-lec-02) | `www/routes/web.php` |
| PHP idioms (`===`, `.`, `->`, `[]`, `require`) | [Lec-10](#lec-10---php-lec-09) | 🐘 notes at the bottom of `drinks.php` |
| PHPDoc `@var` lines in views | [Lec-02](#lec-02---php-lec-01) | `www/views/app/index.php` |
| `preventDefault()` on a form submit | [Lec-19](#lec-19---js-lec-05) | `demo-02.js` |
| Query strings and `$_GET` | [Lec-03](#lec-03---php-lec-02), [Lec-10](#lec-10---php-lec-09) | `/msg?colour=...`; `/drinks` |
| Redirect after POST | [Lec-12](#lec-12---php-lec-11) | `/demo-03/form` |
| Routes (`www/routes/web.php`) | [Lec-02](#lec-02---php-lec-01) | `www/routes/web.php` |
| Search with `LIKE` | [Lec-09](#lec-09---php-lec-08), [Lec-10](#lec-10---php-lec-09) | `/demo/safe`; `/drinks` |
| Sessions (`$_SESSION`) | [Lec-12](#lec-12---php-lec-11), [Auth demo](#authentication-and-authorization-self-study) | `/demo-04/write`, `/demo-04/read` |
| `sort` (JS) | [Lec-17](#lec-17---js-lec-03) | `demo-04.js` |
| Sorting a table by clicking its headers | [Lec-10](#lec-10---php-lec-09) | `/drinks-broken-sort`, `/drinks` |
| SQL injection | [Lec-09](#lec-09---php-lec-08) | `/demo/unsafe-query-read-attack`, `/demo/unsafe-query-write-attack` |
| Sticky form values | [Lec-12](#lec-12---php-lec-11) | `/demo-05/form` |
| Template literals | [Lec-15](#lec-15---js-lec-01) | `demo-04.js` |
| Time zones: store UTC, show local | [Lec-11](#lec-11---php-lec-10) | `/demo-03/time` |
| Truthy, falsy, `===` vs `==` | [Lec-15](#lec-15---js-lec-01) | `demo-05.js` |
| Variables (JS): `const`, `let`, `typeof` | [Lec-15](#lec-15---js-lec-01) | `demo-02.js` |
| Where JavaScript runs | [Lec-15](#lec-15---js-lec-01) | `demo-01.js` |
| XSS (cross-site scripting) | [Lec-09](#lec-09---php-lec-08), [Lec-18](#lec-18---js-lec-04) | `/demo/xss`; `demo-04.js` |

---

## PHP lectures

### Lec-02 - PHP Lec 01

2026-09-09 · Code: [lec-02-php-lec-01-end](https://github.com/MRU-CSIS-3512-001-202604-LEC/lec-02-php-lec-01-end)

- **`/`** - a tour of the framework: routes, controllers and views, and which file does what. Also why every value goes through `e()` before it's echoed, PHPDoc `@var` lines in views, and the 404 page.
- **`/hello`** - adding a route, a controller and a view of your own.

### Lec-03 - PHP Lec 02

2026-09-11 · Code: [lec-03-php-lec-02-end](https://github.com/MRU-CSIS-3512-001-202604-LEC/lec-03-php-lec-02-end)

- **`/msg?colour=...`** - reading a query string through `$_GET`, with `??` supplying a default.
- **`/nmsg/:colour`** - a path parameter, read as `$_GET['colour']`, and `isset()` inside a function of your own.

### Lec-04 - PHP Lec 03

2026-09-14

- **`/callout-demo`** - partials, the simple version: one partial rendered three times with different data.
- **`/team`** - partials, the realistic version: a card partial rendered once per item in a `foreach`. Also an array of associative arrays (the shape a query returns), and an escaping check on a nasty value.
- Files: `www/views/partials/callout.php`, `member-card.php`, `document-head.php`.

### Lec-05 - PHP Lec 04

2026-09-16

- **`/interpolation`** - double vs single quotes, `"$name"` vs `"{$name}"`, and the cases where only the braces work (text after the name, array keys, nested arrays, method calls).
- **`/lab-schedule`** - the alternative syntax for `if` / `elseif` / `else` and `foreach` in a view, an empty-state check, and dates with `DateTimeImmutable`.

### Lec-06 - PHP Lec 05

2026-09-18

The same table of games, shown three ways:

- **`/games-alt-syntax`** - written with the alternative syntax.
- **`/games-std-syntax`** - the same table written with braces, for comparison.
- **`/games-alt-with-partials`** - each table row moved into a partial (`www/views/partials/game-row.php`).

### Lec-07 - PHP Lec 06

2026-09-21 · Code: [lec-07-php-lec-06-end](https://github.com/MRU-CSIS-3512-001-202604-LEC/lec-07-php-lec-06-end)

- **`/games`** - the first database query: a method in `DatabaseQueries`, SQL written as a heredoc, `run()` and `fetchAll()`, and `dd()` to dump what came back.

### Lec-08 - PHP Lec 07

2026-09-23

SQL practice in DB Browser for SQLite. The questions are in `database/lecture/lec-08-analytics-starter.sql` and the worked answers are in `lec-08-analytics-finished.sql`. Each answer shows the wrong attempts too, and why they're wrong.

- `COUNT`, `SUM`, `GROUP BY` and subqueries
- `LEFT JOIN` vs `JOIN`, and where a filter belongs when you `LEFT JOIN`
- `COUNT(*)` vs `COUNT(column)`
- Integer division
- Top 3 with ties kept
- Dates with `strftime()`

### Lec-09 - PHP Lec 08

2026-09-25

- **`/demo/unsafe-query-read-attack`** - SQL injection: a search with user input glued into the SQL, and attacks that dump every row or another table.
- **`/demo/unsafe-query-write-attack`** - SQL injection that changes or destroys data.
- **`/demo/safe`** - the fix: a `:search` named placeholder.
- **`/demo/safe-better`** - the same fix, with the query moved into `DatabaseQueries`.
- **`/demo/xss`** - cross-site scripting: the same input echoed raw and through `e()`.

### Lec-10 - PHP Lec 09

2026-09-28

A drink sales table, built in three stages:

- **`/drinks-starter`** - a plain table from a query with `LEFT JOIN`, `SUM` and `COALESCE`.
- **`/drinks-broken-sort`** - clickable column headers that don't sort, and why: a placeholder can't stand in for a column name or `ASC` / `DESC`.
- **`/drinks`** - search plus sorting done properly: cleaning up `$_GET`, a whitelist for the sort column and direction, and links built in the controller with `http_build_query()`. The 🐘 notes at the bottom of `www/controllers/drinks.php` explain the PHP idioms used.

### Lec-11 - PHP Lec 10

2026-10-02

- **Demo 01: cookie basics** - `/demo-01/set` (a 7-day cookie and a session cookie), `/demo-01/read` (`$_COOKIE`), `/demo-01/clear` (deleting by expiring), `/demo-01/early` ("headers already sent"), `/demo-01/deep/trap` (a cookie set without a path).
- **Demo 02: never trust a cookie** - `/demo-02/join` and `/demo-02/discount`: a discount anyone can give themselves in DevTools.
- **Demo 03: time zones** - `/demo-03/time`: store times in UTC, show them in Edmonton time.

### Lec-12 - PHP Lec 11

2026-10-05

- **Demo 01** - `/demo-01/form`: the same form sent with GET and with POST, and what arrives in `$_GET` and `$_POST`.
- **Demo 02** - `/demo-02/form`: never trust what arrives. Validation on the server (`www/helpers/order.php`), with errors shown in place.
- **Demo 03** - `/demo-03/form`: redirect after POST.
- **Demo 04** - `/demo-04/write` and `/demo-04/read`: sessions, the session id, and its cookie.
- **Demo 05** - `/demo-05/form`: flash messages and sticky values, carried across a redirect.

Lec-13 (PHP Lec 12) finished the Lec-12 material, so it has no repo of its own. Lec-14 was the PHP midterm.

### Authentication and authorization (self-study)

2026-10-07 · Repo: `auth-practice` (accepted through Classroom 50)

Read it with the `authentication-and-authorization-how-to.md` handout in the same repo. Its README has a table of which file shows what.

- **Demo 01** - hashing passwords: `password_hash()` and `password_verify()`.
- **Demo 02** - logging in and out, a restricted page, and a one-time flash message on the login form.
- **Demo 03** - roles: a page and a button only managers can use.

---

## JavaScript lectures

### Lec-15 - JS Lec 01

2026-10-19

- **`/demo-01`** - where it runs: PHP on the server, JavaScript in the browser.
- **`/demo-02`** - values and variables: `const`, `let`, `typeof`, `undefined`.
- **`/demo-03`** - the `+` trap, `Number()` and `NaN`.
- **`/demo-04`** - template literals.
- **`/demo-05`** - truthy and falsy values, and why `===` beats `==`.

### Lec-16 - JS Lec 02

2026-10-21

- **`/demo-01`** - functions are values: declarations, expressions and arrow functions.
- **`/demo-02`** - arrays, indexes and `length`, `for...of`, and why not `for...in`.
- **`/demo-03`** - callbacks and `forEach`.
- **`/demo-04`** - `map`, `filter` and `find`, and what `find` gives back when nothing matches.

### Lec-17 - JS Lec 03

2026-10-23

- **`/demo-01`** - objects: dot and bracket access, and adding properties.
- **`/demo-02`** - objects are shared, not copied, and reassigning a `const`.
- **`/demo-03`** - arrays of objects with `filter`, `map` and `find`, and JSON.
- **`/demo-04`** - `sort`: text order by default, comparing numbers and objects, and how it changes the original array.
- **`/demo-05`** - modules: one entry script per page, `export` and `import`, and how module paths are written.

### Lec-18 - JS Lec 04

2026-10-26

- **`/demo-01`** - selecting from the page: `querySelector`, `querySelectorAll`, changing text, and a selector that matches nothing.
- **`/demo-02`** - creating an element, adding it to the page, and removing one.
- **`/demo-03`** - rendering a list from an array of objects, and emptying it before rendering again.
- **`/demo-04`** - `textContent` vs `innerHTML`, and how `innerHTML` lets a string run as code. `innerHTML` isn't allowed in the Project; this demo shows why.

### Lec-19 - JS Lec 05

2026-10-28

- **`/demo-01`** - listening for a click: `addEventListener`, the event object, changing the page from a listener, and passing a function rather than calling it.
- **`/demo-02`** - submitting a form: a submit listener, the page reload a form does by default, and `preventDefault()` to stop it.
- **`/demo-03`** - reading form fields: `value` from text and number fields (always a string), `checked` from a checkbox, and finding the selected radio button.
- **`/demo-04`** - a form that adds an item to the array from Lec-18 and renders the list again, and the `input` event that fires on every change to a field.
