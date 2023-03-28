![readme-header](https://user-images.githubusercontent.com/1769678/223572353-788d5d38-cd28-40fa-96cd-9d29226f7e4b.png)

<div align="center">

![GitHub License MIT](https://img.shields.io/github/license/wbkd/react-flow?color=%23ff0072)

A highly customizable React component for building interactive flow diagrams.

Coming soon under the MIT licence | Use it now on [isoflow.io](https://isoflow.io)

</div>

## Key Features

- **Real-time:** Display real-time data on diagrams.
- **Customizable:** Use your own isometric icon packs, or use our free set of networking icons (also under MIT).
- **Export options:** Export diagrams as images, JSON or YAML.
- **Powerful annotation tools:** Annotate nodes, groups and connectors.
- **Step-by-step walkthroughs:** Create interactive tours of large diagrams to help viewers easily digest information.

## Roadmap

Migration to open-source: ██░░░░░░░░░

- [x] Set up automated publishing to NPM registry
- [ ] Migrate private JS project to public Typescript project
  - [x] Pan / Select / Zoom modes
  - [x] Display icons in sidebar
  - [ ] Nodes
  - [ ] Groups
  - [ ] Connectors
- [ ] Publish icons as separate importable package

## Installation

Note: Isoflow is currently not production ready. To view it's current state of development:

`npm install isoflow`

```
import Isoflow from 'isoflow';

const App = () => (
  <Isoflow
    height={500}
    scene={{
      icons: [],
      nodes: [],
      connectors: [],
      groups: []
    }}
  >
)
```

If using Next.js, make sure you only import Isoflow in the browser:

```
const Isoflow = dynamic(() => import("isoflow"), {
  ssr: false,
});
```

## License

Isoflow is MIT licensed (see ./LICENSE).
