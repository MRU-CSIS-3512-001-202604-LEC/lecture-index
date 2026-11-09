# Lecture Demo Index - COMP3512-001

**Fall 2026**

![Written by Claude (AI)](https://img.shields.io/badge/written%20by-Claude%20(AI)-D97757?style=for-the-badge)

_This index was written by Claude, an AI assistant made by Anthropic, from the code in each lecture repo._

Trying to remember where you saw something demonstrated? Look it up in the [topic lookup](#topic-lookup), then go to that lecture's section for the routes and files. Lectures are listed newest first.

---

## Where the code is

Each lecture's demo code is in **your own copy** of that lecture's repo, the one you accepted through Classroom 50. Its name ends with the lecture and your GitHub username, like `...-lec-09-php-lec-08-yourusername`.

Three lectures were live-coded, so the finished code is in a public repo instead:

- Lec-07: [lec-07-php-lec-06-end](https://github.com/MRU-CSIS-3512-001-202604-LEC/lec-07-php-lec-06-end)
- Lec-03: [lec-03-php-lec-02-end](https://github.com/MRU-CSIS-3512-001-202604-LEC/lec-03-php-lec-02-end)
- Lec-02: [lec-02-php-lec-01-end](https://github.com/MRU-CSIS-3512-001-202604-LEC/lec-02-php-lec-01-end)

### Running a lecture repo

From the repo's folder:

```
php database/build.php
php -S localhost:8000 -t www/public www/public/index.php
```

Then open http://localhost:8000 and visit the routes listed below. You only need `build.php` for lectures that use the database (Lec-07 onward), and running it again resets the data. From Lec-11 on, the home page links to every demo.

In the JS lectures, the demo files are in `www/public/js/`. Each one is split into numbered STEPs: uncomment one step at a time and watch the console. In the API lectures (Lec-24 and Lec-25), most of the steps are in the PHP files in `www/controllers/api/` instead. From Lec-22 on, the demos read from the fantasy database through JSON endpoints, so run `php database/build.php` first.

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
| `async` and `await` | [Lec-23](#lec-23---js-lec-09) | `demo-01.js` |
| Authentication (logging in and out) | [Auth demo](#authentication-and-authorization-self-study) | `demo-02` |
| Authorization and roles | [Auth demo](#authentication-and-authorization-self-study) | `demo-02`, `demo-03` |
| Bound parameters (named placeholders like `:search`) | [Lec-09](#lec-09---php-lec-08), [Lec-10](#lec-10---php-lec-09) | `/demo/safe`, `/demo/safe-better`; `/drinks` |
| Bubbling: a click travels up through every enclosing element | [Lec-20](#lec-20---js-lec-06) | `demo-01.js` |
| Cache in localStorage: read the copy first, fetch only on a miss | [Lec-26](#lec-26---js-lec-10) | `demo-03.js` STEPs 2-3 |
| Cache kept up to date after a change, and cleared on logout | [Lec-26](#lec-26---js-lec-10) | `demo-03.js` STEPs 5-6 |
| Cache key per user (`inventory:7`, not `inventory`) | [Lec-26](#lec-26---js-lec-10) | `demo-03.js` STEP 4 |
| Callbacks, `forEach` | [Lec-16](#lec-16---js-lec-02) | `demo-03.js` |
| `catch()` at the end of a fetch chain | [Lec-22](#lec-22---js-lec-08) | `demo-04.js` |
| `classList`: add and remove a class, decided from state | [Lec-21](#lec-21---js-lec-07) | `demo-03.js` |
| `COUNT(*)` vs `COUNT(column)` | [Lec-08](#lec-08---php-lec-07) | `lec-08-analytics-finished.sql`, Q2 |
| Controllers vs views | [Lec-02](#lec-02---php-lec-01) | `www/controllers/app/index.php`, `www/views/app/index.php` |
| Cookies: set, read, delete, path | [Lec-11](#lec-11---php-lec-10) | `/demo-01/...` |
| Cookies can't be trusted | [Lec-11](#lec-11---php-lec-10) | `/demo-02/join`, `/demo-02/discount` |
| Data attributes (`data-*`) and `dataset` | [Lec-20](#lec-20---js-lec-06) | `bag-rows.js`, `demo-04.js` |
| `DatabaseQueries` class, `run()` and `fetchAll()` | [Lec-07](#lec-07---php-lec-06), [Lec-09](#lec-09---php-lec-08) | `www/queries/DatabaseQueries.php` |
| Dates and times (`DateTimeImmutable`) | [Lec-05](#lec-05---php-lec-04), [Lec-11](#lec-11---php-lec-10) | `/lab-schedule`; `/demo-03/time` |
| Debugging with `d()` and `dd()` | [Lec-07](#lec-07---php-lec-06), [Lec-10](#lec-10---php-lec-09) | `www/controllers/games.php`; `drinks.php` |
| DELETE request from the page | [Lec-23](#lec-23---js-lec-09), [Lec-25](#lec-25---api-lec-02-recorded) | Lec-23 `demo-04.js`; Lec-25 `demo-02.js` |
| DOM: create, append, remove elements | [Lec-18](#lec-18---js-lec-04) | `demo-02.js` |
| DOM: `querySelector`, `querySelectorAll` | [Lec-18](#lec-18---js-lec-04) | `demo-01.js` |
| DOM: render a list from data | [Lec-18](#lec-18---js-lec-04), [Lec-19](#lec-19---js-lec-05) | Lec-18 `demo-03.js`; Lec-19 `demo-04.js` |
| Empty results: no data, nothing matches, or a list | [Lec-25](#lec-25---api-lec-02-recorded) | `www/controllers/api/merchants.php`, `demo-04.js` |
| Endpoints (PHP): a controller that answers with JSON | [Lec-24](#lec-24---api-lec-01), [Lec-25](#lec-25---api-lec-02-recorded) | `www/routes/api.php`, `www/controllers/api/` |
| Events: `addEventListener` and the event object | [Lec-19](#lec-19---js-lec-05) | `demo-01.js` |
| Events: delegation (one listener for a whole list) | [Lec-20](#lec-20---js-lec-06) | `demo-02.js` (the problem), `demo-03.js` |
| Events: `event.target` and `closest()` | [Lec-20](#lec-20---js-lec-06) | `demo-01.js`, `demo-03.js` |
| Escaping output with `e()` | [Lec-02](#lec-02---php-lec-01), [Lec-04](#lec-04---php-lec-03), [Lec-09](#lec-09---php-lec-08) | home page; `/team`; `/demo/xss` |
| `fetch()` (JS) and Promises: `then()`, `response.json()` | [Lec-22](#lec-22---js-lec-08) | `demo-01.js`, `demo-02.js` |
| `fetch()` vs `fetchAll()` (PDO): one row or a list | [Lec-24](#lec-24---api-lec-01) | `hero_by_id()` in `www/queries/DatabaseQueries.php` (DEMO-1 STEP 3) |
| Flash messages | [Lec-12](#lec-12---php-lec-11), [Auth demo](#authentication-and-authorization-self-study) | `/demo-05/form`; login page |
| Form fields in JS: `value`, `checked`, radio buttons | [Lec-19](#lec-19---js-lec-05) | `demo-03.js` |
| Form validation on the server | [Lec-12](#lec-12---php-lec-11) | `/demo-02/form`, `www/helpers/order.php` |
| Forms: GET vs POST, `$_GET` and `$_POST` | [Lec-12](#lec-12---php-lec-11) | `/demo-01/form` |
| Functions are values (declarations, expressions) | [Lec-16](#lec-16---js-lec-02) | `demo-01.js` |
| "Headers already sent" | [Lec-11](#lec-11---php-lec-10) | `/demo-01/early` |
| `hidden`: show and hide an element, and the CSS `display` rule that beats it | [Lec-21](#lec-21---js-lec-07) | `demo-01.js`; the `[hidden]` rule at the end of `www/public/styles/app.css` |
| `http_response_code()`: 401, 404 and 400 from PHP | [Lec-24](#lec-24---api-lec-01), [Lec-25](#lec-25---api-lec-02-recorded) | Lec-24 `hero.php`, `login.php`; Lec-25 `inventory-delete.php` |
| `innerHTML` vs `textContent` | [Lec-18](#lec-18---js-lec-04) | `demo-04.js` |
| `input` event | [Lec-19](#lec-19---js-lec-05) | `demo-04.js` |
| Interpolation: `"$name"` and `"{$name}"` | [Lec-05](#lec-05---php-lec-04) | `/interpolation` |
| JSON | [Lec-17](#lec-17---js-lec-03) | `demo-03.js` |
| JSON body: reading it in PHP (`php://input`, `json_decode`) | [Lec-24](#lec-24---api-lec-01) | `www/controllers/api/login.php` |
| JSON body: sending a POST from JavaScript | [Lec-23](#lec-23---js-lec-09) | `demo-03.js` |
| `json_encode()` and the `Content-Type` header | [Lec-24](#lec-24---api-lec-01) | `www/controllers/api/hero.php` |
| `LEFT JOIN` and `COALESCE` | [Lec-08](#lec-08---php-lec-07), [Lec-10](#lec-10---php-lec-09) | `database/lecture/` SQL files; `drink_sales_starter()` |
| Links built in the controller (`http_build_query()`) | [Lec-10](#lec-10---php-lec-09) | `www/controllers/drinks.php` |
| localStorage: JSON in and out, and the stored copy is a snapshot | [Lec-26](#lec-26---js-lec-10) | `demo-02.js` |
| localStorage: `setItem`, `getItem`, `removeItem`, and strings only | [Lec-26](#lec-26---js-lec-10) | `demo-01.js` |
| Modules: `import` and `export` | [Lec-17](#lec-17---js-lec-03), [Lec-20](#lec-20---js-lec-06), [Lec-21](#lec-21---js-lec-07) | Lec-17 `demo-05.js`, `demo-05-helpers.js`; Lec-20 `bag-rows.js`; Lec-21 `hero-list.js` |
| `Number()`, `NaN` and the `+` trap | [Lec-15](#lec-15---js-lec-01) | `demo-03.js` |
| Null coalescing (`??`) | [Lec-03](#lec-03---php-lec-02), [Lec-10](#lec-10---php-lec-09), [Lec-25](#lec-25---api-lec-02-recorded) | `www/controllers/msg/index.php`; `drinks.php`; Lec-25 `inventory-delete.php` (DEMO-3 removes it) |
| Objects (JS): dot and bracket access | [Lec-17](#lec-17---js-lec-03) | `demo-01.js` |
| Objects are shared, not copied | [Lec-17](#lec-17---js-lec-03) | `demo-02.js` |
| Partials | [Lec-04](#lec-04---php-lec-03), [Lec-06](#lec-06---php-lec-05) | `/callout-demo`, `/team`; `/games-alt-with-partials` |
| Password hashing | [Auth demo](#authentication-and-authorization-self-study) | `demo-01` |
| Path parameters (`/nmsg/:colour`) | [Lec-03](#lec-03---php-lec-02), [Lec-25](#lec-25---api-lec-02-recorded) | `www/routes/web.php`; Lec-25 `/api/inventory/:item_id` in `www/routes/api.php` |
| PHP idioms (`===`, `.`, `->`, `[]`, `require`) | [Lec-10](#lec-10---php-lec-09) | 🐘 notes at the bottom of `drinks.php` |
| PHPDoc `@var` lines in views | [Lec-02](#lec-02---php-lec-01) | `www/views/app/index.php` |
| `preventDefault()` on a form submit | [Lec-19](#lec-19---js-lec-05) | `demo-02.js` |
| `push()` | [Lec-26](#lec-26---js-lec-10) | `demo-02.js` STEP 2 |
| Query string in a fetch URL | [Lec-22](#lec-22---js-lec-08) | `demo-04.js` |
| Query strings and `$_GET` | [Lec-03](#lec-03---php-lec-02), [Lec-10](#lec-10---php-lec-09) | `/msg?colour=...`; `/drinks` |
| Redirect after POST | [Lec-12](#lec-12---php-lec-11) | `/demo-03/form` |
| Remove an item: change the array, then render again | [Lec-20](#lec-20---js-lec-06) | `demo-04.js` |
| `response.ok`: a 404 is a reply, not a failure | [Lec-23](#lec-23---js-lec-09) | `demo-02.js` |
| Routes (`www/routes/web.php`) | [Lec-02](#lec-02---php-lec-01) | `www/routes/web.php` |
| `rowCount()`: how many rows a DELETE removed | [Lec-25](#lec-25---api-lec-02-recorded) | `remove_from_inventory()`, `inventory-delete.php` (DEMO-1) |
| Search with `LIKE` | [Lec-09](#lec-09---php-lec-08), [Lec-10](#lec-10---php-lec-09) | `/demo/safe`; `/drinks` |
| Sessions (`$_SESSION`) | [Lec-12](#lec-12---php-lec-11), [Auth demo](#authentication-and-authorization-self-study) | `/demo-04/write`, `/demo-04/read` |
| `sort` (JS) | [Lec-17](#lec-17---js-lec-03) | `demo-04.js` |
| Sorting a table by clicking its headers | [Lec-10](#lec-10---php-lec-09) | `/drinks-broken-sort`, `/drinks` |
| SQL injection | [Lec-09](#lec-09---php-lec-08) | `/demo/unsafe-query-read-attack`, `/demo/unsafe-query-write-attack` |
| State: one page, many views, drawn from a few variables | [Lec-21](#lec-21---js-lec-07) | `demo-02.js` |
| Sticky form values | [Lec-12](#lec-12---php-lec-11) | `/demo-05/form` |
| Template literals | [Lec-15](#lec-15---js-lec-01) | `demo-04.js` |
| Templates (`<template>`): repeated markup, `cloneNode(true)` | [Lec-21](#lec-21---js-lec-07), [Lec-22](#lec-22---js-lec-08) | Lec-21 `demo-04.js`, `www/views/demo-04.php`; Lec-22 `demo-04.js` |
| Time zones: store UTC, show local | [Lec-11](#lec-11---php-lec-10) | `/demo-03/time` |
| Truthy, falsy, `===` vs `==` | [Lec-15](#lec-15---js-lec-01) | `demo-05.js` |
| `try` / `catch` around `await` | [Lec-23](#lec-23---js-lec-09) | `demo-02.js` |
| Validating an endpoint's input (400) | [Lec-25](#lec-25---api-lec-02-recorded) | `www/controllers/api/inventory-delete.php` (DEMO-3) |
| Validating markup your JavaScript built (duplicate ids) | [Lec-21](#lec-21---js-lec-07) | `demo-04.js` STEP 3 |
| `var_dump` in an endpoint: read it in the Response tab | [Lec-24](#lec-24---api-lec-01), [Lec-25](#lec-25---api-lec-02-recorded) | Lec-24 `login.php` (DEMO-3); Lec-25 `inventory-delete.php` (DEMO-1 STEP 1) |
| Variables (JS): `const`, `let`, `typeof` | [Lec-15](#lec-15---js-lec-01) | `demo-02.js` |
| Where JavaScript runs | [Lec-15](#lec-15---js-lec-01) | `demo-01.js` |
| XSS (cross-site scripting) | [Lec-09](#lec-09---php-lec-08), [Lec-18](#lec-18---js-lec-04) | `/demo/xss`; `demo-04.js` |
---

## JavaScript and API lectures

### Lec-26 - JS Lec 10

2026-11-16

The Network tab and the Application panel (Storage, Local storage) do most of the explaining today. To start a demo fresh, clear Local storage there.

- **`/demo-01`** - localStorage keeps strings and only strings: a number comes back as text (`"11" + 1` is `"111"`), an object is stored as `"[object Object]"`, and a key that isn't there gives `null`.
- **`/demo-02`** - storing an object as JSON and parsing it back. The stored text is a snapshot: changing the object afterwards with `push()` doesn't change what's stored.
- **`/demo-03`** - caching a hero's bag: STEP 2 stores a copy after the fetch, STEP 3 reads the copy first and skips the request on a hit, STEP 4 fixes the key so one hero can't see another's bag, STEP 5 updates the copy after a drop, STEP 6 removes it on logout. STEP 4 is a one-line edit in `cacheKey()`, described in the file's header. The page shows the cache key and where the bag came from.

### Lec-25 - API Lec 02 (recorded)

2026-11-13 · Five video clips instead of a live lecture

Most steps are in the PHP files in `www/controllers/api/`; each file's header lists them in order. Run `php database/build.php` to get dropped items back.

- **`/demo-01`** - `DELETE /api/inventory/:item_id`, built step by step and tested from the Console: the path's value lands in `$_GET`, and `rowCount()` of 0 means a 404.
- **`/demo-02`** - the same DELETE from a Drop button: the database changes when the server says yes, and the page only changes when your code changes the array.
- **`/demo-03`** - the DELETE with no `hero_id`: a PHP warning breaks the JSON, then a 400 before the query runs.
- **`/demo-04`** - `GET /api/merchants/:item_id`: an empty array can't tell two of the three cases apart, so the JSON has to.

### Lec-24 - API Lec 01

2026-11-09

The steps are in the PHP files, `www/controllers/api/hero.php` and `login.php`, and each file's header lists them in order. The pages' JavaScript is finished.

- **`/demo-01`** - `GET /api/hero?id=7`, built step by step: `echo` can't print an array, `json_encode()` can, then `fetch()` vs `fetchAll()` and the `Content-Type` header.
- **`/demo-02`** - `GET /api/hero?id=999`: with no row, the unfixed endpoint answers `false` with status 200. Then `http_response_code()` and a JSON error.
- **`/demo-03`** - `POST /api/login`: `$_POST` is empty for a JSON body, so read `php://input` and `json_decode()` it, then answer with an id or a 401.

### Lec-23 - JS Lec 09

2026-11-06

- **`/demo-01`** - Wednesday's `then` chain rewritten with `async` and `await`: `await` pauses the function, not the page, and an `async` function hands back a Promise. Comment STEP 1's chain out before you uncomment STEP 2, as the file's header says.
- **`/demo-02`** - `try` / `catch` around `await`, a missing `await`, and two kinds of 404: a JSON error and the framework's HTML page. The file's header lists the live edits in order.
- **`/demo-03`** - a login form that POSTs a JSON body: a known email moves to the character sheet, an unknown one stays on the form with a message. Look at the request's Payload tab.
- **`/demo-04`** - a DELETE request from a Drop button, then the array changes and the list renders again. (Not reached in lecture; the Lec-25 recording covers it.) Run `php database/build.php` to get dropped items back.

### Lec-22 - JS Lec 08

2026-11-04

- **`/demo-01`** - `fetch()` doesn't wait: it hands back a Promise right away, and `then()` says what to do with the response when it arrives.
- **`/demo-02`** - two waits: the response, then `response.json()` for the body, chained with two `then`s; and why keeping what `fetch()` hands back gives you a Promise, not the data.
- **`/demo-03`** - the Lec-21 hero views with the heroes from `/api/heroes`: building the list right after calling `fetch()` finds no heroes, so it moves inside the `then`. Comment STEP 1's last block out before you uncomment STEP 2, as the file's header says.
- **`/demo-04`** - one slot's items, asked for with a query string (`/api/items?slot=head`) and drawn with a `<template>`, and a `catch()` for when no reply comes back.

### Lec-21 - JS Lec 07

2026-11-02

- **`/demo-01`** - hiding an element with `hidden`, and why it fails on an element whose CSS sets `display` (here `display: flex`). STEP 3 is not in the JS file: it's the commented-out `[hidden] { display: none !important; }` rule at the end of `www/public/styles/app.css`.
- **`/demo-02`** - one page, two views: the state is two `let` variables, `render()` hides every view and shows the one the state names, and every click changes the state and then calls `render()`. Try changing the starting values to `"sheet"` and `7` and reloading. The heroes come from `hero-list.js`, a module this demo and the next share.
- **`/demo-03`** - marking the chosen hero with `classList`: STEP 1 adds the class straight onto the page and ends up marking two heroes; STEP 2 keeps the choice in a variable and lets the render function decide. Comment STEP 1's listener out again before you uncomment STEP 2, as the file's header says.
- **`/demo-04`** - building rows from a `<template>`: a template's contents aren't on the page, then clone, find the `li` in the copy, fill it with `textContent`, append it. STEP 3 shows why a template must never hold an `id`: two copies give two elements with the same id, which the W3C validator reports as an error.

### Lec-20 - JS Lec 06

2026-10-30

- **`/demo-01`** - bubbling: a click on a button is heard by the button and by every element around it, innermost first, and `event.target` says what was actually clicked.
- **`/demo-02`** - one listener per row, and why it fails: a row added later, or rebuilt by rendering again, has no listener. The rows come from `bag-rows.js`, a module the next two demos share.
- **`/demo-03`** - event delegation: one listener on the list, `closest("button")` to find the clicked button even when the click lands on its icon, and rows added later working too.
- **`/demo-04`** - reading the item's id from `data-item-id` with `dataset` (always a string), then removing the item from the array and rendering the list again.

### Lec-19 - JS Lec 05

2026-10-28

- **`/demo-01`** - listening for a click: `addEventListener`, the event object, changing the page from a listener, and passing a function rather than calling it.
- **`/demo-02`** - submitting a form: a submit listener, the page reload a form does by default, and `preventDefault()` to stop it.
- **`/demo-03`** - reading form fields: `value` from text and number fields (always a string), `checked` from a checkbox, and finding the selected radio button.
- **`/demo-04`** - a form that adds an item to the array from Lec-18 and renders the list again, and the `input` event that fires on every change to a field.

### Lec-18 - JS Lec 04

2026-10-26

- **`/demo-01`** - selecting from the page: `querySelector`, `querySelectorAll`, changing text, and a selector that matches nothing.
- **`/demo-02`** - creating an element, adding it to the page, and removing one.
- **`/demo-03`** - rendering a list from an array of objects, and emptying it before rendering again.
- **`/demo-04`** - `textContent` vs `innerHTML`, and how `innerHTML` lets a string run as code. `innerHTML` isn't allowed in the Project; this demo shows why.

### Lec-17 - JS Lec 03

2026-10-23

- **`/demo-01`** - objects: dot and bracket access, and adding properties.
- **`/demo-02`** - objects are shared, not copied, and reassigning a `const`.
- **`/demo-03`** - arrays of objects with `filter`, `map` and `find`, and JSON.
- **`/demo-04`** - `sort`: text order by default, comparing numbers and objects, and how it changes the original array.
- **`/demo-05`** - modules: one entry script per page, `export` and `import`, and how module paths are written.

### Lec-16 - JS Lec 02

2026-10-21

- **`/demo-01`** - functions are values: declarations, expressions and arrow functions.
- **`/demo-02`** - arrays, indexes and `length`, `for...of`, and why not `for...in`.
- **`/demo-03`** - callbacks and `forEach`.
- **`/demo-04`** - `map`, `filter` and `find`, and what `find` gives back when nothing matches.

### Lec-15 - JS Lec 01

2026-10-19

- **`/demo-01`** - where it runs: PHP on the server, JavaScript in the browser.
- **`/demo-02`** - values and variables: `const`, `let`, `typeof`, `undefined`.
- **`/demo-03`** - the `+` trap, `Number()` and `NaN`.
- **`/demo-04`** - template literals.
- **`/demo-05`** - truthy and falsy values, and why `===` beats `==`.

---

## PHP lectures

### Authentication and authorization (self-study)

2026-10-07 · Repo: `auth-practice` (accepted through Classroom 50)

Read it with the `authentication-and-authorization-how-to.md` handout in the same repo. Its README has a table of which file shows what.

- **Demo 01** - hashing passwords: `password_hash()` and `password_verify()`.
- **Demo 02** - logging in and out, a restricted page, and a one-time flash message on the login form.
- **Demo 03** - roles: a page and a button only managers can use.

### Lec-12 - PHP Lec 11

2026-10-05

- **Demo 01** - `/demo-01/form`: the same form sent with GET and with POST, and what arrives in `$_GET` and `$_POST`.
- **Demo 02** - `/demo-02/form`: never trust what arrives. Validation on the server (`www/helpers/order.php`), with errors shown in place.
- **Demo 03** - `/demo-03/form`: redirect after POST.
- **Demo 04** - `/demo-04/write` and `/demo-04/read`: sessions, the session id, and its cookie.
- **Demo 05** - `/demo-05/form`: flash messages and sticky values, carried across a redirect.

Lec-13 (PHP Lec 12) finished the Lec-12 material, so it has no repo of its own. Lec-14 was the PHP midterm.

### Lec-11 - PHP Lec 10

2026-10-02

- **Demo 01: cookie basics** - `/demo-01/set` (a 7-day cookie and a session cookie), `/demo-01/read` (`$_COOKIE`), `/demo-01/clear` (deleting by expiring), `/demo-01/early` ("headers already sent"), `/demo-01/deep/trap` (a cookie set without a path).
- **Demo 02: never trust a cookie** - `/demo-02/join` and `/demo-02/discount`: a discount anyone can give themselves in DevTools.
- **Demo 03: time zones** - `/demo-03/time`: store times in UTC, show them in Edmonton time.

### Lec-10 - PHP Lec 09

2026-09-28

A drink sales table, built in three stages:

- **`/drinks-starter`** - a plain table from a query with `LEFT JOIN`, `SUM` and `COALESCE`.
- **`/drinks-broken-sort`** - clickable column headers that don't sort, and why: a placeholder can't stand in for a column name or `ASC` / `DESC`.
- **`/drinks`** - search plus sorting done properly: cleaning up `$_GET`, a whitelist for the sort column and direction, and links built in the controller with `http_build_query()`. The 🐘 notes at the bottom of `www/controllers/drinks.php` explain the PHP idioms used.

### Lec-09 - PHP Lec 08

2026-09-25

- **`/demo/unsafe-query-read-attack`** - SQL injection: a search with user input glued into the SQL, and attacks that dump every row or another table.
- **`/demo/unsafe-query-write-attack`** - SQL injection that changes or destroys data.
- **`/demo/safe`** - the fix: a `:search` named placeholder.
- **`/demo/safe-better`** - the same fix, with the query moved into `DatabaseQueries`.
- **`/demo/xss`** - cross-site scripting: the same input echoed raw and through `e()`.

### Lec-08 - PHP Lec 07

2026-09-23

SQL practice in DB Browser for SQLite. The questions are in `database/lecture/lec-08-analytics-starter.sql` and the worked answers are in `lec-08-analytics-finished.sql`. Each answer shows the wrong attempts too, and why they're wrong.

- `COUNT`, `SUM`, `GROUP BY` and subqueries
- `LEFT JOIN` vs `JOIN`, and where a filter belongs when you `LEFT JOIN`
- `COUNT(*)` vs `COUNT(column)`
- Integer division
- Top 3 with ties kept
- Dates with `strftime()`

### Lec-07 - PHP Lec 06

2026-09-21 · Code: [lec-07-php-lec-06-end](https://github.com/MRU-CSIS-3512-001-202604-LEC/lec-07-php-lec-06-end)

- **`/games`** - the first database query: a method in `DatabaseQueries`, SQL written as a heredoc, `run()` and `fetchAll()`, and `dd()` to dump what came back.

### Lec-06 - PHP Lec 05

2026-09-18

The same table of games, shown three ways:

- **`/games-alt-syntax`** - written with the alternative syntax.
- **`/games-std-syntax`** - the same table written with braces, for comparison.
- **`/games-alt-with-partials`** - each table row moved into a partial (`www/views/partials/game-row.php`).

### Lec-05 - PHP Lec 04

2026-09-16

- **`/interpolation`** - double vs single quotes, `"$name"` vs `"{$name}"`, and the cases where only the braces work (text after the name, array keys, nested arrays, method calls).
- **`/lab-schedule`** - the alternative syntax for `if` / `elseif` / `else` and `foreach` in a view, an empty-state check, and dates with `DateTimeImmutable`.

### Lec-04 - PHP Lec 03

2026-09-14

- **`/callout-demo`** - partials, the simple version: one partial rendered three times with different data.
- **`/team`** - partials, the realistic version: a card partial rendered once per item in a `foreach`. Also an array of associative arrays (the shape a query returns), and an escaping check on a nasty value.
- Files: `www/views/partials/callout.php`, `member-card.php`, `document-head.php`.

### Lec-03 - PHP Lec 02

2026-09-11 · Code: [lec-03-php-lec-02-end](https://github.com/MRU-CSIS-3512-001-202604-LEC/lec-03-php-lec-02-end)

- **`/msg?colour=...`** - reading a query string through `$_GET`, with `??` supplying a default.
- **`/nmsg/:colour`** - a path parameter, read as `$_GET['colour']`, and `isset()` inside a function of your own.

### Lec-02 - PHP Lec 01

2026-09-09 · Code: [lec-02-php-lec-01-end](https://github.com/MRU-CSIS-3512-001-202604-LEC/lec-02-php-lec-01-end)

- **`/`** - a tour of the framework: routes, controllers and views, and which file does what. Also why every value goes through `e()` before it's echoed, PHPDoc `@var` lines in views, and the 404 page.
- **`/hello`** - adding a route, a controller and a view of your own.
