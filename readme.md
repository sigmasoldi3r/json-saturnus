# JSON Saturnus

A simple library written in Saturnus for parsing and serializing JSON data.

Just add this line to your `[dependencies]` section:
```toml
json = { git = "https://github.com/sigmasoldi3r/json-saturnus" }
```

Example:
```rs
use json;

let object = { example: "Object", a: [1, 2, 3] };

let str = json.stringify(object, 2);
print(str);

let o = json.parse(str);
print("Example:", o.example);
```
