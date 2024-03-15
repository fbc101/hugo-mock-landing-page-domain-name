# hugo-mock-landing-page

This repository was made as a homework assignment for CIS 3500. The website shows the prototype of a product. In this case, CrimeGuard, is a map application with the ability to consider ongoing crimes and previous criminal data when determining the path to a destination.

The workflow pages-deployment.yaml updates the deployment of the website whenever there is a push on the main branch. To be more specific "on: push: branches: - main" tells the GitHub Actions workflow to run the jobs defined in it whenever there is a push event to the main branch of the repository. 

So, after changes are made to the  Hugo website source files and push those changes to the main branch, this workflow will automatically:
- Check out the latest code
- Set up the Hugo environment
- Build the static website files by running hugo
- Publish the built files to the gh-pages branch

The gh-pages branch is then used by GitHub Pages to serve/deploy the updated website.
