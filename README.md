# ies-snippets README

React Snippets 的基本集合

- rbase react base template

```ts
import React from "react";

type TProps = {};
export const T: React.FC<TProps> = (props) => {
  return <div></div>;
};
```

- rfc react function components

```ts
type TProps = {};
const T: React.FC<TProps> = (props) => {
  return <div></div>;
};
```

- rsc subject context

```ts
import { BaseContext, transferable } from "@ies/ic-common-subject-context";

type State = {};
@transferable
export class Context extends BaseContext<State> {
  constructor() {
    super({});
  }

  setState(state: Partial<State>) {
    this.dispatch({
      ...state,
    });
  }
}
```
