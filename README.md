# Active Archives Initiative 
> The official website of the Active Archives Initiative. Built using Jekyll and Prose by [@blms](https://github.com/blms).


## Contents 
- [Posts](#posts)
- [News section](#news-section)
- [Miscellaneous](#miscellaneous)


## Posts
Posts may be created, edited, and deleted with [Prose](https://prose.io).
Once authenticated, click on the `mitaai` Group on the right panel, and then enter the `mitaai.github.io` Project.

There are two kinds of posts with different metadata structures: Team pages, which are special profile pages for team members; 
and Blog posts, which encompass all other types of posts.

You will notice there is a directory structure including `aai-news`, `projects`, `research`, and `team`. These directories only exist
to distinguish between Team pages and all other types of posts (i.e. Blog posts). They will affect which metadata structure you may use.


### Blog posts

Create a new Blog post by selecting `New File` inside the `aai-news`, `projects`, or `research` directory. Click the Metadata
icon on the right sidebar to edit metadata. This should be fairly self-explanatory, but there are a few important notes:

- **Category**: The category you select determines which page the post shows up under. You may select multiple categories, and the post will appear
on multiple pages. If you wish for the post to also show up on the front page grid, please also add the "show on front page grid" 
category. The most recent posts will appear first on the front page.

- **Thumbnail**: If you wish to add a thumbnail image to the grid on the front page and/or on the category page (projects, research, etc), you may
either upload an image on GitHub to the `/assets/images` directory, or simply use an external image URL. If you choose to upload an image,
you must enter the URL as such: `/assets/images/marginalia.jpg` (for example).

- **Header image**: You may also add a header image to the post, with a few different styling options. This must be added separately from the 
Thumbnail. The same image upload rules as the Thumbnail apply, and it works best with large images, with a width of at least 1000px. **Note**: 
It is highly recommended that you also add a caption. 

- **Image style/crop position**: These options only take effect if a Header image exists. Feel free to play around with these styling options 
until you get the desired result. 

Additional images and other formatting may be added with Prose's built-in editor.


### Team pages

Create a new Team page by selecting `New File` inside the `team` directory. Click the Metadata icon on the right sidebar to edit metadata. This 
should be fairly self-explanatory, but there are a couple of important notes:

- **Thumbnail**: Team member pages automatically embed the thumbnail into the body of the document, [like so](https://aai.mit.edu/2015-02-03-kurt-fendt). 
There is no need to add an additional image.

- **Category**: You will notice there is no "Category" metadata option here. That is because all Team pages are automatically assigned to the `team` category.
If you wish to showcase a team member on the front page, it is recommended that you make a blog post in the `aai-news` category, separate from their Team 
profile page.


## News section

To add or remove items from the News section, please edit the file `_data/front-news.yml`. Each entry must be in the following 
format, with indentation:
```yml
- title: Active Archives Initiative launches new website
  url: /2020-02-10-aai-website
  date: 2020-02-02
```
or, for external links:
```yml
- title: Activist artists hack New Museum visitors' poll
  url:  https://news.artnet.com/art-world/hans-haacke-museum-hack-1759014
  date: 2020-01-22
```


## Miscellaneous

The Newsletter blurb can be edited in the file `/newsletter.markdown`.
