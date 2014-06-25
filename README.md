# Levenshtein-steps

[Levenshtein][wikipedia] string difference in Javascript.

![Screenshot][screenshot]

`Levenshtein-steps` also does some neat things like coerce to a number and string
approproately. So you can compare Levenshtein objects directly! Not to mention
it has specs!

Also it tells you the steps to get from one string to another.


## API

* `new Levenshtein( m, n )` → `Levenshtein`
    * m ( `String` ): First string.
    * n ( `String` ): Second string.
    * Initialise a new Levenshtein object.

* `Levenshtein#distance` → `Number`
    * Distance between strings.

* `Levenshtein#inspect()` → `String`
    * Pretty print Levenshtein table.

* `Levenshtein#toString()` → `String`
    * Alias of: `Levenshtein#inspect()`.

* `Levenshtein#valueOf()` → `Number`
    * Alias of: `Levenshtein#distance`.
    
* `Levenshtein#getSteps()` -> `Array[Array]`
    * Returns list of the steps to get from string 1 to string 2
    * Steps in form of lists - `["operation", int_pos_str_1, int_pos_str_2]`


## Installation

Levenshtein works in both the browser and [node.js][node].


### Browser

Simply include `levenshtein.js`:

``` html
<script src="/javascripts/levenshtein.js"></script>
```


### NPM

Install via npm:

``` sh
npm install levenshtein-steps
```

Or put it in your `package.json`:

``` json
{ "levenshtein-steps": "*" }
```


### Bower

``` sh
bower install levenshtein-steps
```


### Git

``` sh
git clone git://github.com/pseudonym117/Levenshtein.git
```


## License

Levenshtein-steps is [UNLICENSED][unlicense].


## Author

Written by [Gianni Chiappetta][github] &ndash; [gf3.ca][gf3]

Forked and steps added by [AG Stephan][mygit]


[gf3]: http://gf3.ca
[github]: https://github.com/gf3
[node]: http://nodejs.org/
[screenshot]: http://f.cl.ly/items/3g1m0u401j0m2H2k0s2X/levenshtein.PNG
[unlicense]: http://unlicense.org/
[wikipedia]: http://en.wikipedia.org/wiki/Levenshtein_distance
[mygit]: https://github.com/pseudonym117
