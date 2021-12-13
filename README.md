# Supabase Svelte Kanban with Snowpack deployed on Vercel

A [Trello](https://trello.com) clone using [Supabase](https://supabase.io) as the storage system.

https://github.com/supabase-community/svelte-kanban

https://github.com/coding-to-music/svelte-kanban

https://svelte-kanban-gamma.vercel.app/

## [Click Here for Live Demo of Svelte Supabase Kanban](https://supabase-kanban.vercel.app/)

### Screenshot

![Screenshot](https://github.com/coding-to-music/svelte-kanban/blob/main/screenshot.png?raw=true)

# Setup locally

1. Clone the repo with `gh repo clone joshnuss/supabase-kanban` and install dependencies with `yarn install`
2. Setup the database on [supabase](https://supabase.io) and run the commands in [`setup.sql`](https://github.com/joshnuss/supabase-kanban/blob/master/setup.sql)
3. Update the credentials in `.env.development`
4. Install dependancies `yarn install`

Output
```java
warning ../package.json: No license field
[1/4] Resolving packages...
[2/4] Fetching packages...
[3/4] Linking dependencies...
warning "eslint-plugin-jest > @typescript-eslint/experimental-utils > @typescript-eslint/typescript-estree > tsutils@3.19.1" has unmet peer dependency "typescript@>=2.8.0 || >= 3.2.0-dev || >= 3.3.0-dev || >= 3.4.0-dev || >= 3.5.0-dev || >= 3.6.0-dev || >= 3.6.0-beta || >= 3.7.0-dev || >= 3.7.0-beta".
[4/4] Building fresh packages...
Done in 68.44s.
```

5. Start development server with `yarn start`

Output
```java
yarn run v1.22.17
warning ../package.json: No license field
$ snowpack dev --polyfill-node
[snowpack] ! installing dependencies...
[snowpack] ✔ install complete! [4.64s]
[snowpack] 
  ⦿ web_modules/                                size       gzip       brotli   
    ├─ @supabase/supabase-js.js                 132.17 KB  28.53 KB   23.97 KB   
    ├─ gravatar-url.js                          15.61 KB   4.68 KB    3.83 KB    
    ├─ svelte-dnd-action.js                     79.5 KB    18.41 KB   15.69 KB   
    ├─ svelte-hmr/runtime/hot-api-esm.js        22.46 KB   7.5 KB     6.37 KB    
    ├─ svelte-hmr/runtime/proxy-adapter-dom.js  5.43 KB    1.72 KB    1.42 KB    
    ├─ svelte.js                                0.21 KB    0.16 KB    0.12 KB    
    ├─ svelte/animate.js                        0.86 KB    0.4 KB     0.35 KB    
    ├─ svelte/easing.js                         3.94 KB    1.07 KB    0.95 KB    
    ├─ svelte/internal.js                       54.84 KB   13.84 KB   11.94 KB   
    ├─ svelte/store.js                          3.3 KB     1 KB       0.88 KB    
    ├─ svelte/transition.js                     6.79 KB    2.09 KB    1.76 KB    
    └─ tinro.js                                 6.7 KB     2.93 KB    2.64 KB    
  ⦿ web_modules/common/ (Shared)
    └─ _commonjsHelpers-eb5a497e.js             0.67 KB    0.33 KB    0.27 KB    

  http://localhost:8080 
  Server started.


[eslint] > Watching src
```
6. Done!

## Available Scripts

### yarn start

Runs the app in the development mode.
Open http://localhost:8080 to view it in the browser.

The page will reload if you make edits.
You will also see any lint errors in the console.

### yarn test

Runs `jest` on all `*.test.js` files.

### yarn lint

Runs `eslint` on all files.

### yarn format

Formats all files according to rules defined in `.eslintrc.js`.

### yarn build

Builds a static copy of your site to the `build/` folder.
Your app is ready to be deployed!

### yarn deploy

Deploys the app to [vercel](https://vercel.com)

# License

MIT
