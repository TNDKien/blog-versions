# blog-versions

These are the versions of the blog project that I have created.
## First iteration: Making the blog

### [Version 1: Sidebar Navigation from v0](./Blog%20V1)

Used v0 to create a homepage and sidebar navigation for the blog. Since the rest of the blog it created was not what I wanted, I decided to start over with just the sidebar navigation.


### [Version 2: Basic Blog Setup](./Blog%20V2)

Created a basic blog setup with a homepage and sidebar navigation in Storyblok. Making sure the sidebar is seperated from the content.
#### Changelog:
- Added components: Blog, BlogContainer, BlogTeaser
- Added blog/[slug] for blog pages


## Second Iteration: Changing the tutorial blog to one that will focus on research as well

### [Version 3: Functionality with Article Pages](./Blog%20V3)

Created a components for articles with similar setup as the blog components, updating whenever a new article is created. This is something I've learned from a previous project.
#### Changelog:
- Added components: Article, ArticleContainer, ArticleTeaser
- Added article/[slug] for Article pages


### [Version 4: Comment System](./Blog%20V4)

I've asked for feedback on the blog to my teachers and they suggested making a blog about the things I like. After that, I was looking around at other blogs checking out what topics they were discussing and what kind of blogs were posted. I came across blogs that were more like researches/articles focusing on trending and certain topics within the dev community. Addidionally I noticed that they had a comment system. I wanted to add one to my blog, but I didn't know how to do it. So I asked v0 to create a comment system for the blog. Using an API route to save the comments to a JSON file. I've tested it in the local environment and it works, but found out it doesn't work in the production environment when hosted on Vercel.
#### Changelog:
- created an api/comments/route.ts to post, save and get comments
- added a data folder with an empty comment.json where the comments get stored in
- added a lib/ui/comment-section.tsx


## Third Iteration: Changing the way of storing data from the JSON within the project to a database

### [Version 5: Comment system with Supabase](./Blog%20V5)

In this version, I've asked with chatGPT for suggestions on other ways to make a comment system. It suggested using a database to save the comments. I've created a database in Supabase and connected it to the blog. I've also created a comment component that shows the comments for an article.
#### Changelog:
- created a database in Supabase
- added Supabase url and key in the .env.local to connect with the database
- updated the api/comments/route.ts to match with the Supabase database instead of the JSON file


