to setup a tailwind project:

step 1:
npm init

step 2:
npm i tailwindcss postcss-cli autoprefixer

step 3:
npx tailwind init

step 3:
postcss.config.js

module.exports = {
plugins: [require("tailwindcss"), require("autoprefixer")],
};

step 4:
css/tailwind.css

@tailwind base;
@tailwind componnents;
@tailwind utilities;

step 5:
package.json > scripts :

"build": "postcss css/tailwind.css -o public/build/tailwind.css"

step 6:
npm run build

step 7:
Add css Link to index.html boilerplate

<link rel="stylesheet" href="./public/build/tailwind.css" />

step 8:
Happy Coding!
