# Example site: netlify-plugin-form-submissions

This site only exists to demonstrate a Netlify Build Plugin.

- Learn more about the [netlify-plugin-form-submissions](https://github.com/philhawksworth/netlify-plugin-form-submissions) plugin.
- See this example site here: https://demo-netlify-plugin-form-submissions.netlify.app


## Quick try-out

You can try out this site and its plugin out by deploying it.

Clicking the button below will clone this repo, setup a new site [on Netlify](https://netlify.com?utm_source=github&&utm_medium=plugin-formsubmissions-pnh&utm_campaign=devex) and deploy the site complete with the plugin configured and operational.

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/philhawksworth/demo-netlify-plugin-form-submissions&utm_source=github&utm_medium=plugin-formsubmissions-pnh&utm_campaign=devex)

## Configuration



```toml
...

# Config for the Netlify Build Plugin: netlify-plugin-form-submissions
[[plugins]]
  package = "netlify-plugin-form-submissions"

  [plugins.inputs]
    # Get submissions for specific forms
    # e.g. "form-name"
    # e.g. ["form-name-1", "form-name-2"]
    # e.g. "ALL"
    # default: "ALL"
    formNames = "ALL"

    # the folder to recieve json files for each form
    dataDirectory = "src/_data"


```

