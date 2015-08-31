# Sureup Backend Exercise
Goals: Build an api to serve a list of Year Make and Model combinations.

Go to [http://developer.edmunds.com/](http://developer.edmunds.com/) and sign up for an api key.

Build a server that responds to:

`GET` `/vehicles/year.json`

and returns an `array` of years available ( as strings ) i.e.
```
[
  '2012',
  '2013',
  '...'
]
```

---

`GET` `/vehicles/2012/make.json`

Which returns an array of all the `manufactures` who made cars in `2012`

```
[
 'Honda',
 'Toyota',
 'Ford',
 '...'
]
```

---

`GET` `/vehicles/2012/toyota/models.json`

Which returns all the models made by `Toyota` in `2012`.

```
[
  'Celica',
    'Camry',
    '...'
]
```

---

`GET` `/vehicles/2012/toyota/camry/trim.json`

Which returns the different trims a `2012` `Toyota` `Camry` was made in.

```
[
 'XLE',
 'LE',
 '...'
]
```

---

`GET` `/vehicles/2012/toyota/camry/xle/price.json`

Which returns the price of a 2012 Toyota Camry.

Let's pretend our API is `awesomely` popular and we get `5000` hits per second. `Edmunds` is now rate limiting us which affects our users. How would you solve this problem?

