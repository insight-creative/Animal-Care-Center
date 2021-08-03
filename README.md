# Animal Care Center of Buffalo Grove

A custom Hugo website built from the Insight Creative, Inc. Hugo starter boilerplate Quintessence. The [Hugo](https://gohugo.io/) boilerplate we use for our projects.

The repo for the boilerplate can be found at https://github.com/insight-creative/Quintessence

**Disclaimer** - This site has been heavily integrated with [Netlify](https://www.netlify.com/), and therefore many features are specific to the Netlify platform and may not work with other hosting providers. This site also uses [NetlifyCMS](https://www.netlifycms.org/) as a CMS. Make sure to run a git pull before starting any work in case the client has made changes on their end. 

## Getting Started

To get started, clone the repository, then run the following from the project root:

```
npm install
hugo server
```

Simple as that, you can now start building everything you need. Hugo's server has automatic SCSS and JS processing through their Hugo Pipes system. Read more about that in their docs.

## File Structure

```
│   │
|   └──── /assets            - Source files for assets (SCSS, JS etc)
|   | cricital.scss          - css file that gets injected inline into the head so we can load our critical styles faster and delay the rest until they are needed
|   | dark.scss              - css file that holds styles for anyone that has dark mode preferences set on their devices
|   | main.scss              - css file that holds all our main styles
│
|
└──── /content               - Content files
|   | about                  - About page content and assets
|   | careers                - Careers page content and assets
|   | contact                - Contact page content and assets
|   | request-appointment    - Request Appointment page content and assets
|   | services               - Services page content and assets
|   | thank-you              - Thank You page content and assets
|   | _index.md              - Home page content
|
└──── /data                  - Data files,  business_info.yml holds our basic business info
|
└──── /layouts               - Template files
│   │ _default               - Here you will find the base template, baseof.html along with a generic list and single template.
│   │ about                  - About Page template
│   │ careers                - Careers Page template
│   │ contact                - Contact Page template
│   │ partials               - Partials are any reusable bits of code or in some cases larger section like head.html that are broken out to keep code easier to manage 
│   │ request-appointment    - Request Appointment Template
│   │ services               - Services Templates, both single and list templates live in here
│   │ shortcodes             - No special shortcodes were needed for this site
│   │ sitemap                - Sitemap Template, this is the human readable sitemap. For this site, we do not have one.
│   │ thank-you              - Thank You Template
│   │ 404.html               - 404 Template
│   │ home.html              - Homepage Template
│   │ index.headers          - Custom Netlify HTTP headers
│   │ index.redirects        - Custom Netlify redirect rules
│   │ robots.txt             - Template for robots.txt
│   │ sitemap.xml            - Sitemap
│   │
│   └──── /_default          - Base templates for list & singular pages
│   │   │ baseof.html        - Base template
│   │   │ list.html          - List/taxonomy template
│   │   │ single.html        - Singular page/post template
│   │
│   └──── /partials          - Partials
│   |   │ footer.html        - Sites primary <footer>
│   |   │ head.html          - Sites primary head section, containing SEO data, stylesheet configurations and more
│   |   │ header.html        - Sites primary <header>
│   |   │ cta.html           - Sites primary cta block
│   |   │ scripts.html       - Sites primary scripts and JS processing/pipes setup
│   │
│   └──── /static            - Hugo static resources
|       | admin              - Configuration for Netlify CMS
|       | images             - A few static images like the site logo can be found here. Most images are stored in their page bundles
│
│ .gitignore
│ LICENSE
│ README.md
│ config.toml                - Hugo configuration, probably the most important piece in here is the navigation menu
│ postcss.config.js          - PostCSS and PurgeCSS configuration for Hugo Pipes
│ netlify.toml               - Netlify configuration
│ package.json
```

The above File Structure should give you a pretty good understanding of where everything is if/when changes are needed.

All content is editable through the CMS except for the services icons. The client has access to this as well. Make sure to always do a git pull before starting any work on the site in case they have been in the CMS and made any updates on their end.

There's really not a whole lot more too it. Happy building!
