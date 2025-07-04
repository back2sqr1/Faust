# Common Matchers

## Comparison by exact equality

```ts
test('two plus two is four', () => {
  expect(2 + 2).toBe(4);
});
```

```ts
test('object assignment', () => {
  const data = {one: 1};
  data['two'] = 2;
  expect(data).toEqual({one: 1, two: 2});
});
```

- `toEqual` ignores object keys with `undefined` properties, `undefined` array items, array sparseness, or object type mismatch. To take these into account use `toStrictEqual` instead.

## Describe

`describe(name, fn)` creates a block that groups together several related tests. For example, if you have a `myBeverage` object that is supposed to be delicious but not sour, you could test it with: