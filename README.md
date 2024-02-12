### Setting up a New Website

**Step 1: Create a New Site**

To begin, navigate to GitHub and select "Use this template" to create a new repository based on the just-the-docs template. Name the repository something like "doc-appname" or "doc-companyname-appname".

**Step 2: Configure Repository Settings**

In the repository settings, under the "Pages" section, ensure that the branch set for publishing is "main" and the folder is set to "root".

**Step 3: Clone the Repository**

Next, using GitHub Desktop or another tool of your choice, clone the newly created repository to your local machine.

**Step 4: Set Up a Development Branch**

Create a new branch named "development" within GitHub Desktop. Switch to this branch and make your initial commit labeled as "Version 0".

**Step 5: Edit Content with Obsidian**

Open Obsidian and open the folder where your new repository is located. Adjust the layout using the includes, layout, and sass folders provided. For instance, you can modify the sidebar's background color in light.scss and customize the sidebar's footer in sidebar.html.

### Writing Content

- Ensure that each new note includes the frontmatter property "layout: home" and a header (e.g., # Header line) to be displayed properly.
- Keep drafts in the designated "Drafts" folder to maintain organization. Move notes out of this folder to make them visible on the live server.
- To organize notes under collections, move them into folders named according to the collection (e.g., _ChapterOne). Ensure that the collection folder starts with an underscore and that the "output:true" attribute is set in the config.yml file.
- Adjust the config.yml file to create or rename collections. Note that changes to config.yml require restarting the Jekyll server to take effect.

### Publishing

Merge changes from the development branch into the main branch, using a descriptive commit message (e.g., "Version 1"). Sync the changes to GitHub and wait for the website to go online. You can access it at https://yourusername.github.io/repositoryname.

### Additional Information

- The helpers folder contains useful resources such as a markdown cheatsheet and configuration instructions for the "just-the-docs" template.
- Preview changes locally by running "jekyll serve watch" in the root of your vault. This command starts a Jekyll server at localhost:4000, allowing you to see how the website will look once synced with GitHub.
- Various Obsidian plugins are installed to assist with managing the vault and its contents, including Clear Unused Images, Shell Commands, Consistent Attachment and Links, File Hider, Git, Commander, Templater, and Editing Toolbar.