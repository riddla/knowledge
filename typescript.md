---
description: How Do I ...
---

# TypeScript

## ... import \(typed JSON files\)?

```typescript
declare module "*.json" {
    const value: any;
    export default value;
}
```

Source: [https://github.com/aurelia/cli/issues/493\#issuecomment-281916899](https://github.com/aurelia/cli/issues/493#issuecomment-281916899)

## Have you had a chance to answer the previous question?

Yes, after a few months we finally found the answer. Sadly, Mike is on vacations right now so I'm afraid we are not able to provide the answer at this point.



