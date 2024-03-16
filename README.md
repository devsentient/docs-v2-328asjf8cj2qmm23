# docs-v2-328asjf8cj2qmm23

# Overview
[Public documentation page](https://docs.hyperplane.dev/docs-v2-328asjf8cj2qmm23/#/) to guide users in using the Shakudo Platform. Uses [docsify](https://github.com/docsifyjs/docsify/) to generate the page. 

# Adding additional documentation
1. Copy or create your markdown file of the desired page into the `./docs` directory (or in a sub directory for organization i.e. `./docs/introduction`
 for deployment docs)
1. Then add the page to `./docs/_sidebar.md`. 
1. If the page has links to other notion pages or uses local files/images, then they must be added to the /docs folder, and the links in the markdown file must be updated.
    1. For child pages
        1. Add the markdown file to the `./docs` directory the same way as above.
        1. Ensure the parent page's markdown file links to these child pages from the root directory `./docs`.
    1. For local files/images:
        1. Place them anywhere in the `./docs` directory i.e. `./docs/images` for general images used in pages.
        1. Ensure that the page that uses local content uses the link to these files/images relative to the current page's path i.e. a markdown file in `./docs/introduction` may want to use images by linking to `images/some_picture.png` (which has an absolute path of `./docs/introduction/images/some_picture.png`)
1. Upon merge to the main branch, any changes should be reflected within a few minutes and displayed on (the page)[https://docs.hyperplane.dev/docs-v2-328asjf8cj2qmm23]

Note: You can embed HTML elements/tags within markdown files to support more custom styling.

# Testing Locally
Follow the steps on the [docsify docs](https://docsify.js.org/#/quickstart) to serve and test the page locally.
