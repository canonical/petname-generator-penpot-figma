# Canonical pet name generator plugin for Figma and Penpot
<img src="https://github.com/user-attachments/assets/f7eef9f3-c5d0-4d59-8525-ea97a4d33770" width="600">

This is a plugin which can generate Ubuntu style pet names for selected text nodes in Figma and Penpot.

## Building

To build the plugins run `npm run build`. This will create a `dist` folder. Follow [Figmas](https://www.figma.com/plugin-docs/plugin-quickstart-guide/) and [Penpots](https://help.penpot.app/plugins/create-a-plugin/#2.7.-step-7.-load-the-plugin-in-penpot) on how to locally import these build plugins.

## Development

This is esentially a React app. Both plugins share most of their code. They just need different plugin Typescript files which are located under `./src/plugin/` and different manifest files located under `./plugin-manifests`.
The vite config contains different build modes for the HTML and Javascript for both Figma and Penpot. Executing `npm run build` runs all of them.

The contents of the public folder are required by the Penpot plugin.
