```js
import * as d3 from "npm:d3";

import { FileAttachment } from "npm:@observablehq/stdlib";
```

```js
const gistemp = FileAttachment("/releases/Release 1/Brain_V1.csv")
  .csv({ array: true, typed: true })
  .then((data) => {
    console.log(data.length);
  });
```

<h1>New</h1>
