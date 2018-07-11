# TypeScript

## Import \(typed JSON files\)

```typescript
declare module '*.json' {
  const value: JSON;
  export default value;
}

export type JSONObject = { [key: string]: JSON };
export interface JSONArray extends Array<JSON> {}
export type JSON = null | string | number | boolean | JSONArray | JSONObject;
```

### Sources

{% embed data="{\"url\":\"https://github.com/aurelia/cli/issues/493\#issuecomment-281916899\",\"type\":\"link\",\"title\":\"Typescript error \\\"TS2307: Cannot find module \'../aurelia.json\'\\\" within build tasks · Issue \#493 · aurelia/cli\",\"description\":\"I&\#39;m submitting a bug report \(i guess\)  Library Version: 1.0.8  Please tell us about your environment:   Operating System: Windows 10   Node Version: 6.9.4   NPM Version: 4.1.1   Browser: Not Br...\",\"icon\":{\"type\":\"icon\",\"url\":\"https://github.com/fluidicon.png\",\"aspectRatio\":0},\"thumbnail\":{\"type\":\"thumbnail\",\"url\":\"https://avatars3.githubusercontent.com/u/2870365?s=400&v=4\",\"width\":420,\"height\":420,\"aspectRatio\":1}}" %}

{% embed data="{\"url\":\"https://github.com/Microsoft/TypeScript/issues/15225\#issuecomment-294718709 \",\"type\":\"link\",\"title\":\"JSON.parse\(\) returns any, but should return Object · Issue \#15225 · Microsoft/TypeScript\",\"description\":\"TypeScript Version: 2.3.0 Expected behavior: JSON.parse\(\) should return Object, as stated in MDN. Actual behavior: JSON.parse\(\) returns any, essentially getting rid of the useful compile-time type ...\",\"icon\":{\"type\":\"icon\",\"url\":\"https://github.com/fluidicon.png\",\"aspectRatio\":0},\"thumbnail\":{\"type\":\"thumbnail\",\"url\":\"https://avatars3.githubusercontent.com/u/3440331?s=400&v=4\",\"width\":400,\"height\":400,\"aspectRatio\":1}}" %}

## Type object keys

```typescript
const criteria1 = Symbol();
const criteria2 = Symbol();
const criteria3 = Symbol();

interface gridFilter {
  [criteria1]: string[];
  [criteria2]: string[];
  [criteria3]: string[];
}
```

Source: [https://www.typescriptlang.org/docs/handbook/symbols.html](https://www.typescriptlang.org/docs/handbook/symbols.html)

