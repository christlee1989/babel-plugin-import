# babel-plugin-import-component

修改样式引入规则

----

## Example

#### `{ "libraryName": "antd", style: "css" }`

```javascript
import { Button } from 'pandora-mobile';
<Button>xxxx</Button>

      ↓ ↓ ↓ ↓ ↓ ↓
      
var _button = require('pandora-mobile/lib/button');
require('pandora-mobile/lib/button/style/index.css');
<_button>xxxx</_button>
```

#### `{ "libraryName": "antd", style: true }`

```javascript
import { Button } from 'pandora-mobile';
<Button>xxxx</Button>

      ↓ ↓ ↓ ↓ ↓ ↓
      
var _button = require('pandora-mobile/lib/button');
require('pandora-mobile/lib/button/style/index.scss');
<_button>xxxx</_button>
```
