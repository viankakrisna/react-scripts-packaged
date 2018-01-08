An experiment to package https://github.com/facebookincubator/create-react-app react-scripts to an executable package using https://github.com/zeit/pkg to ensure that the setup always works regardless of your environment.
Right now it only supports 64-bit machines and packages node 8 inside it.

How to use:
- download the executable for your os 
- put the file at the root of your create-react-app generated project
- update your package.json scripts section (this is for macos, update the name of the package according your machine):
  - `react-scripts start` to `./react-scripts-packaged-macos start`
  - `react-scripts build` to `./react-scripts-packaged-macos build`
  - `react-scripts test --env=jsdom` to `./react-scripts-packaged-macos test --env=jsdom`

Feel free to report any bugs or pr for improvements!