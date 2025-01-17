# Usage

## Remember to update "custom domain" field after running `npm run publish`

## Deploy to GitHub Pages

Before you deploy, commit your changes to any working branch except the `gh-pages` one and run the following command:

    npm run publish

**Important note**: Chalk does not support the standard way of Jekyll hosting on GitHub Pages. You need to deploy your working branch (can be any branch, for xxx.github.io users: use another branch than `master`) with the `npm run publish` command. Reason for this is because Chalk uses Jekyll plugins that aren't supported by GitHub pages. The `npm run publish` command will automatically build the entire project, then push it to the `gh-pages` branch of your repo. The script creates that branch for you so no need to create it yourself. Also, if you are developing a **project site**, you must set the `baseurl` in `_config.yml` to the name of your repository.

You can find more info on how to use the `gh-pages` branch and a custom domain [here](https://help.github.com/articles/quick-start-setting-up-a-custom-domain/).

[View this](https://github.com/nielsenramon/kickster#automated-deployment-with-circle-ci) for more info about automated deployment with Circle CI.

### Installation

If you haven't installed the following tools then go ahead and do so (make sure you have [Homebrew](https://brew.sh/) installed):

    brew install ruby
    brew install npm

On windows, install Ruby and Node with the installers found here:

  - [Ruby](https://rubyinstaller.org/)
  - [Node.js](https://nodejs.org/en/download/)

Next setup your environment:

    npm run setup

### Development

Run Jekyll:

    npm run local
