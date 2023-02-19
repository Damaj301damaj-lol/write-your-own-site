# sitemap.xml
This file is also not required, however this will make the job of search engine crawlers easier to find your site's data, here is an example of a sitemap.xml file:
```xml
<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  <url>
    <loc>https://example.com/</loc>
    <lastmod>2020-01-01</lastmod>
    <changefreq>monthly</changefreq>
    <priority>0.8</priority>
  </url>
  <url>
    <loc>https://example.com/about</loc>
    <lastmod>2020-01-01</lastmod>
    <changefreq>monthly</changefreq>
    <priority>0.8</priority>
  </url>
  <url>
    <loc>https://example.com/contact</loc>
    <lastmod>2020-01-01</lastmod>
    <changefreq>monthly</changefreq>
    <priority>0.8</priority>
  </url>
  ```
This is a very basic sitemap.xml file, it has 3 pages, the homepage, the about page, and the contact page, you can add as many pages as you want, just make sure to add the `<url>` tag, and the `<loc>` tag, the `<loc>` tag is the url of the page, the `<lastmod>` tag is the last time the page was modified, the `<changefreq>` tag is how often the page is updated, and the `<priority>` tag is the priority of the page, the higher the number, the more important the page is.

You can also add a `<sitemap>` tag, which is a link to another sitemap.xml file, this is useful if you have a lot of pages, and you don't want to have a huge sitemap.xml file, you can split it up into multiple files, and link them together.
