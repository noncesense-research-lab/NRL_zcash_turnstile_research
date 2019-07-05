# Zcash Turnstile
A [Noncesense Research Lab](http://www.noncesense.org) study by [Isthmus](https://www.github.com/mitchellpkt) (Mitchell Krawiec-Thayer, Ph.D.)

Modeling ZIP 308 ([Proposal](https://github.com/zcash/zips/pull/197), [Discussion](https://github.com/zcash/zips/pull/197))

```
The amount to send in each transaction is chosen according to the 
following distribution:

1. Choose an integer exponent uniformly in the range 6 to 9 inclusive. [UPDATE: max 8]
2. Choose an integer mantissa uniformly in the range 1 to 99 inclusive.
3. Calculate amount := (mantissa * 10:sup:`exponent`) zatoshi.
4. If amount is greater than the amount remaining to send, repeat from step 1.
```

See figures and notes in Jupyter Notebook