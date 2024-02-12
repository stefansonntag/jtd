This repo serves a template to create a new Github pages website for documentations, specifically those that would to be called from within a Qlik app to show inline help. It uses the just-the-docs template/just-the-docs template remote template.  

### Set up a new site

1) In GitHub click "Use template". and give the new repo a a name like "doc-appname" or "doc-companyname-appname".
2) Go to settings of the new repo under "pages" and ensure that you set the branch from which to publish to "main" and folder "root" 
3) Open GitHub Desktop and add a new local repo by selecting "clone" and then choose from github.com the repo created in step 1. Obviously that could also be done somehow in VSCode or by using the Git CLI "clone" command, but I found it the easiest to use GitHub Desktop 
4) Create a new branch in GitHub Desktop (again: could be done also in any other tool) and call it ""development". This will copy all the content from the "main" branch into your new branch. Make sure you switch to that new branch before you start to edit, then create a first commit, call it Version 0 and publish that new development branch to GitHub.
5) Open Obsidian and use the open vault command to open the folder in which your new repo from step one resides. Confirm that you trust the author of the vault so that the plugins get activated.
6) Adapt the layout, use the incudes, layout and sass folder. The background color for the sidebar is defined as white in light.scss under sass/color_schemes. The omission of the default footer in the sidebar ("Built with just-the-docs") is done in includes/components/sidebar.html, at the very end between the footer and /footer tags.
### Write content
1) Create a new note and start writing. A frontmatter property "layout: home" needs to be in the note and a # header line or else local jekyll or github pages will not show the note!
2) New notes will be created automatically in the "Drafts" folder to keep the vault clean. There is already a note called "My 1st Page" in that folder to get started. Move it to some other place to see it in the live server because the drafts folder is excluded from publication by Jekyll / GitHub pages!
3) To put a note under a collection (e.g. First Capter) , move it into the name of the  folder that is specified in config.yml as the collection folder (e.g. _ChapterOne). 
4) IMPORTANT: Collection folder need to start with an underscore and in config.yml there need to be an attribute "output:true"
5) To create a new collection (e.g. Chapter Three), change the config.yml file under "collections:". Any change to config.yml will require to restart the jekyll server to become visible (e.g. renaming collections or adding new ones)
6) **<font color="#ff0000">**Do not forget to commit intermittently to save versions of your doc to the development branch!**</font>

### Publish
Merge the development branch into the main branch, commit (use a version name as commit message, e.g. "Version 1", synch it to GitHub and wait 1-2 minutes until the website comes online. You can see it subsequently at https://stefansonntag.com/changeforyournewreponame. Also you can go to the new repo in GitHub and click on actions and see how the GitHub build process runs
   
### Other
The helpers folder contains two notes
   1) a markdown cheatsheet
   2) a link to the configuration instruction for the template "just the docs" which is used to generate the web site. Read it to understand which other tempaltes for template you could create, e.g. parent child templates, note with table of contents etc
   
When you run "jekyll serve watch" (I use a terminal window in VSCode ) in the vault root you can point a browser to "localhost:4000" and see how the website will look like once synched with GitHub. Running the command will keep a jekyll server up at port 4000 which can obviously be done only once. So if the command fails the most likely reason is that the port is already blocked by another instance of a jekyll server. To mitigate do a "ps" and kill -9 that server and rerun 'jekyll serve'

### Vault configuration

The following Obsidian plugins are installed in the vault:
   1) Clear Unused Images (removes screenshots etc which aren'r referenced anymore)
   2) Shell commands. not configured for anything specific set, but just in case you want to be able to execute a command line program (e.g. git, jekyll etc.) in the vaults directory
   3) Consistent Attachment and Links: help to clean the vault clean. Specifically it will create a folder "attachments" in the same directory where a screenshot is pasted into an article and move it into that folder. If you move the article into any other directory the plugin will do the same in the new directory and update the link in the doc. Comes very handy!
   4) File hider: Configures to hide the "_site" folder in the vault that Jekyll creates when you run "jekyll serve"
   5) Git. All kinds of Git commands are available via the Obsidian command palette (search for git). Most handy comes a) creation of a new branch (switches to that new branch immediately) and b) commit to current branch
   6) Commander: allows to fix command palette commands to toolbars, menus etc so that they can be executed without  the need to topen the palette with "CMD p" and then search
   7) Templater: to configure a template which gets created when creating a new note. This is currently the simplest one which adds a property "layout: home" to the front matter
   8) Editing Toolbar: apply markdown syntax easily by using icons in the note editor


