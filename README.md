# Create a Beautiful Documentation Website for your Github Project

Here are the steps for creating a documentation website for your Github project 
using Github Pages. These steps are super quick and easy and require ZERO
coding!

## Prerequisites

1. Create an acccount on [github.com](https://github.com/)
2. Create a new Github repository or select an existing repository to hold your
new documentation website

## Step 1. Navigate to Github Pages in your repository's settings

To get to your repository's Github Pages settings, head over to your 
repository's **Settings**, then select **Pages** from the left sidebar.

## Step 2. Set up the "source" for your documentation website

According to Github, the "source" for your documentation website can be one of
two things:
* A branch (Easy Option) 
* A Github Actions Workflow (Hard Option)

For this tutorial, we'll go with the Easy Option (a branch). This means you'll 
need to...
1. Set **Source** to **Deploy from a branch**
2. Set **Branch** to the branch you want to deploy from (e.g., **`main`**)
3. Select which folder in your chosen branch will hold your website's files 
(if you want to host your website at the root of your branch, select 
**`/(root)`**)
4. Click **Save**

## Step 3. Add your documentation

Initialize a `README.md` file in the EXACT location where you set your 
Github Pages site to deploy from in the previous step.

For example, if you set your source branch to **`main`** and your source 
directory to **`/(root)`**, place your `README.md` file at the root of your 
`main` branch.

**Note:** Make sure to add some nice content to your new README file and be 
sure to commit and push this `README.md` file so you can see it in
your remote repository on Github.

## Step 4. Verify your "barebones" documentation site is up-and-running

Navigate to `https://{your_username}.github.io/{your_repository_name}` in your
web browser and verify your site is up and running. Be sure to replace 
`{your_username}` with your Github username and `{your_repository_name}` with 
the name of your Github repository.

You should see the contents of your README file on your website.

## Step 5. "Beautify" your website by adding a Jekyll Theme

1. Initialize a `_config.yml` file in the EXACT location where you set your 
Github Pages site to deploy from in **Step 2**. For example, if you set your 
source branch to **`main`** and your source directory to **`/(root)`**, place 
your `_config.yml` file at the root of your `main` branch.
2. Pick a theme from Github's [list of supported themes](https://pages.github.com/themes/)
3. Open your `_config.yml` and type the following line:
`theme: jekyll-theme-{theme-name}` (be sure to replace `{theme_name}` with your
chosen theme's name). For example, if I chose the Hacker Theme, I'd put the this
line in my `_config.yml` file:
`theme: jekyll-theme-hacker`
4. Commit and push your `_config.yml` file.

Now, navigate back to `https://{your_username}.github.io/{your_repository_name}` 
in your web browser and verify that your site is now styled with your chosen
theme!