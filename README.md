# NodeCDN
A simple library that transforms JavaScript into a better platform.

## Installation
- For client sides: `<script class="nodecdn-init" src="https://hostereric.herokuapp.com/NodeCDN/init/index.min.js"></script>`
- For backend: Go down to the [backend section](https://github.com/WWEMGamer2/NodeCDN/blob/main/README.md#initialising-on-the-backend).

## Initialising on the backend
- Python (Flask):
  `pip install nodecdn` or use your Package Manager to search for `nodecdn`.
  
## For standalone installs:
1. Download the latest ZIP file from [Releases](https://github.com/WWEMGamer2/NodeCDN/releases/tag/StandaloneInstalls)
2. UnZIP, then move to your website's asset directory
3. Initialise it like in this example here (change the src to your corresponding path): `<script class="nodecdn-init standalone" src="assets/NodeCDN/init/index.min.js"></script>`

## Start coding
- To initialise in JavaScript, copy and paste this code into your script file:
```javascript
nd = new Node(); //initialise the NodeCDN minimal js script
nd.Client('key'); //initialise the client

Init();
```

- To initalise in Python, copy and paste this code into your script files:
```python
# This is the file where your Flask server will be

from flask import Flask
from nodecdn import backend, frontend

app = Flask('app')

@app.route('/')
def index(): return "home"

backend.init(app);
app.run()
```

```html
<!--Put before body tag -->
<script src="nodecdn/dist"></script>
<script>

</script>
```
