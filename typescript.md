# TypeScript

## Import \(typed JSON files\)

```typescript
declare module "*.json" {
    const value: any;
    export default value;
}
```

Source: [https://github.com/aurelia/cli/issues/493\#issuecomment-281916899](https://github.com/aurelia/cli/issues/493#issuecomment-281916899)

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

