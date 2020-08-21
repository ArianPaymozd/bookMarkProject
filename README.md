# bookMarkProject

# Firstly we install dependencies for Webpack:

npm install webpack webpack-cli

# Secondly we create a config file for webpack:

webpack.config.js

# On your webconfig file:
We need to setup a configuration for webpack. Reading below;
The entry file will be the main source (which imports and loads other source files). I used index.js as mine.
Then Web pack will generate a source file named "main.js" during build.
I also configured a path to where webpack will generate and save "main.js".

module.exports = {
    entry: './src/index.js',
    output: {
      filename: 'main.js',
      path: path.resolve(__dirname, 'public'),
      library: 'mainLib',
    },
  };
