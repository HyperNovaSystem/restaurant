# Restaurant

**▶ Live demo: https://hypernovasystem.github.io/restaurant/**

A real-time restaurant simulation built with
[DOMECS](https://github.com/HyperNovaSystem/domecs).

## Features
- Customers arrive at the restaurant, wait to be seated, eat, and leave.
- Waiters seat customers, take orders, serve food, and clear tables.
- The restaurant has a limited number of tables and waiters, so customers may have to wait.
- The restaurant can be configured with different numbers of tables, waiters, and customer arrival rates.
- The simulation runs in real-time and can be paused/resumed.

---

## Local development

This app depends on the DOMECS runtime packages via `file:../domecs/packages/*`,
so clone it **alongside** the [`domecs`](https://github.com/HyperNovaSystem/domecs)
repo:

```sh
# C:\dev\HyperNova\
#   ├─ domecs/
#   └─ restaurant/   <- here
npm install
npm test          # tsc --noEmit && vitest
npm run dev        # play in the browser
npm run deploy     # vite build + publish dist/ to the gh-pages branch
```

Built with DOMECS — an ECS-driven DOM engine. Extracted from the DOMECS
`example/` suite into its own repo.
