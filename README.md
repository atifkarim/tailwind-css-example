# tailwind-css-example
This project helps to learn Tailwind CSS as a beginner

# Installation process

- Install from CDN (Not possible to customize Tailwind CSS)
- Install as PostCSS plugin
- Install Tailwind CLI
  - It helps to use Tailwind using command line

## Prerequisite to Install Tailwind CLI

- Node.js version must be `>12.3.0`

## Necessary commands

- At first create the directory where tailwindcss will be developed
- Configure a node project: `npm init -y`
- Install tailwindcss as developer dependency: `npm i -D tailwindcss`
- Instal tailwind css [VSCode plugin](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss)
- Create configuration file for tailwindcss: `npx tailwindcss init`. This will create a file which helps to create a file where all configure and customize related to tailwindcss is possible
- Create `src` and `outout` folder.
  - `src` folder will contain tailwindcss files. Create a file inside this and give any name with `.css` extension
  - `output` folder will contain compiled vanilla/raw css file

- Later, created `.vscode/settings.json` file
- Now, Add build scripts in `package.json` file
  ```sh
  "scripts": {
    "build": "tailwindcss -i ./src/tailwind.css -o ./output/tailwind.css -w",
  }
  ```
  Here, `i` means input. Then input and output directory is pointed. `-w` for watch which helps to automate the build process

## Minutes about TailwindCSS

- This is a Utility-First Approach, while Bootstrap is a Component approach