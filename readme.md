## For fun project, never use this lol

a scrappy json parser implementation following https://lihautan.com/json-parser-with-javascript/

Added implementation for parsing BigInt & symbol with new syntax:

```
  {
    "bigInt": +0x1fffffffffffff+,
    "symbol": $Heyy$
  }
```
returns

```js
{
  bigInt: 9007199254740991n,
  symbol: Symbol(Heyy) 
}
```
