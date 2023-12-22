# kiwojtylak.github.io
[![pages-build-deployment](https://github.com/kiwojtylak/kiwojtylak.github.io/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/kiwojtylak/kiwojtylak.github.io/actions/workflows/pages/pages-build-deployment) 

[kiwojtylak.github.io](https://kiwojtylak.github.io) is the public website of Katarzyna (Kasia) I. Wojtylak

## How is this site built
This site is hosted on Gitlab Pages, and built using one of the Jekyll community templates. Jekyll allows to generate a static website, from markdown pages and SCSS.  
The main branch of the repository remains blank, and the repository is organized around different branches, each for a different Jekyll theme.
The site is published from the corresponding theme branch.

## Template structure  
The site is structured in components for the different concerns: contents (markdown), structure (html layouts), and styles (SCSS).  
Original files have been renamed to start with underscore (ie: README.md to _README.md) instead of deleting or editing on top.  
The structure for the currently configured theme is as follows:
```markdown
.
├── 📁 assets
│   ├── 📁 css
│   │   ├── *.scss: 
│   ├── 📁 favicon
│   │   ├── *.png: 
│   ├── 📁 img
│   │   ├── 📁 portfolio
│   │   │   ├── *.jpg: 
│   │   ├── 📁 timeline
│   │   │   └── *.png: 
│   │   ├── *.png: 
│   └── 📁 js
│       ├── *.js
├── 📁 _data
│   ├── navigation.yml: 
│   ├── sitetext.yml: 
│   └── style.yml: 
├── 📁 docs
│   └── *.png: 
├── 📁 _includes
│   ├── *.html
├── 📁 _layouts
│   ├── *.html
├── 📁 _portfolio
│   ├── *.md
├── 📁 _sass
│   ├── 📁 base
│   │   ├── *.scss
│   ├── 📁 components
│   │   ├── *.scss
│   └── 📁 layout
│       ├── *.scss
├── .gitattributes: configures the main programming language of this repository
├── .gitignore: gitignore file for local development
├── 404.html: 
├── BACKLOG.md: 
├── CNAME: 
├── _config.yml: 
├── Gemfile: 
├── Gemfile.lock: 
├── index.md: 
├── jekyll-agency.gemspec: 
├── legal.md:
├── README.md: 
└── run.sh:
```

404.md: markdown page to display if a page is not found
BACKLOG.md: backlog of the latest tasks and bugfixes
CNAME: github generated file for custom domain configuration
Gemfile: configuration about Jekyll plug-ins
README.me: this file
_config.yml: basic site attributes, like the currently configured theme, the hosting URL, tittle (displayed in several places), contact e-mail, description, author, selected locale, Google Analytics tracking code, or whether the portfolio section is displayed
index.md: entrypoint layout.
jekyll-agency.gemspec: specifications for Jekyll runtime and dependencies
legal.md: markdown page for the "Privacy" section
run.sh: this script allows to run the site for local development

## Developing
Editing from local environment  facilitates development with all the conveniences provided by an IDE (ie: PyCharm).  
Changes done locally can be tested by running generating and serving the site locally, using the run.sh script. 
For the site to run locally, Jekyll and Bundle need to be installed on the machine.
Ready to ship changes, can be commited & pushed to the remote Github repository either by the correspondent IDE tool, or by git commands on the command-line.  

For small changes, it is also possible to edit and commit the files from the Github web interface.  

## Publishing changes
gh action

## Custom domain
custom domain