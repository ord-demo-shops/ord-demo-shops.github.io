# Fictional demo shops for the Open Resolution Desk

This repository serves two fictional shops on GitHub Pages:

- Brackenlight Home, lamps and ceramics: https://ord-demo-shops.github.io/brackenlight/
- Coppice Cycles, wheel builds and parts: https://ord-demo-shops.github.io/coppice/

They exist to show the Open Resolution Desk
(https://taronsung.github.io/open-resolution-desk/) working across independent
websites. No products, payments or deliveries are real, and the names are
invented for the demo.

Each shop is an open agentic website. It publishes:

- `agent-manifest.json` with its assistant network and a `resolution` block
  that names its terms versions, its offers, its representative and the desk
- `terms/v*.json`, its returns terms as data, every version kept
- `agents/agent-manifest.json` and a representative network that other sites
  load by URL
- `backoffice.html`, the page where the shop checks a case from the desk with
  its own records before it confirms

The files here are generated. Their sources, the build script and the tests are
in https://github.com/taronsung/open-resolution-desk (`src/shops`). Rebuild
with `npm run publish:prod` in that repository.

License: Apache License 2.0. The browser runtime in each `runtime/` folder comes
from the agentic-web repository under the same license.
