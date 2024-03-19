# Planet Keeper Hack the Weave submission

### Troubles

- tailwind docs do not list one step of adding the new index.css file as an import to the main.tsx file
- SQL addition being accepted by vercel
- the wallet connect import did not work, so I had to use their actual template to add the Arweave wallet connect functionaltiy
- the wallet connect functionality works on the desktop, but not on the mobile so far.

```

  <script type="module" src="/sqlite/main.js"></script>
  <pre class="main"></pre>
  <pre class="worker"></pre>

```

### Building roadmap

- [x] Start new template
- [x] desktop Arweave wallet connect functionality
- [x] mobile Arweave wallet connect functionality
- [x] test SQLite
  - result: worked locally did not pass through vercel so could not include it
- [] aos PlanetKeeper chatroom
- [x] create beekeeper token and .lua file
  - templates are made but not tested yet
- [] tokengate PlanetKeeper chatroom
- [] upload the website to Arweave to create a full stack Arweave app.
- [] tutorial video

```

function Prompt()
    return "PlanetKeeper@aos> "
end

```

- [] potential --cron (30-minutes)
- [] Understaning Process Ownership
  Start a new process with the aos console, the ownership of the process is set to your wallet address. aos uses the Owner global variable to define the ownership of the process. If you wish to transfer ownership or lock the process so that no one can own, you simply modify the Owner variable to another wallet address or set it to nil.

- [] encoding data as json
  When sending data to another process or an external service, you may want to use JSON as a way to encode the data for recipients. Using the json module in lua, you can encode and decode pure lua tables that contain values.

lua
Send({Target = Router, Data = require('json').encode({hello = "world"})})

- [] upload the website to Arweave to create a full stack Arweave app.

### Lessons Learned

Tutorials can be most effective when the knowledge is given at a tempo or pace. We built ours so that each user fully absorbs that step before being able
to move on to the next step. This interactivity creates a more engaging learning experience that can be more effective than traditional methods.
