# TypeScript

## Import \(typed JSON files\)?

```typescript
declare module "*.json" {
    const value: any;
    export default value;
}
```

Source: [https://github.com/aurelia/cli/issues/493\#issuecomment-281916899](https://github.com/aurelia/cli/issues/493#issuecomment-281916899)

