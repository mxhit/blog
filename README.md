## Blog

The blog is hosted at [mxhit.github.io](https://mxhit.github.io/).

### Steps for making a post

1. Create a new post in the `content/posts/` directory with the following command
```
hugo new posts/{file-name}.md
```

2. Change the value of `draft` to `false` in `{file-name}.md` once blog content has been added in the file.
```
---
title: "File Name"
date: 2022-05-29T18:12:45+05:30
draft: false
---
```

3. Create static assets of the blog post.
```
hugo -t PaperMod
```

4. Navigate to `public/` directory to commit all the files and eventually push them to the [repo](https://github.com/mxhit/mxhit.github.io).
```
cd public/
git add .
git commit -m "Commit message goes here"
git push origin main
```

5. Post should be reflected on the blog after a few seconds on [mxhit.github.io](https://mxhit.github.io/).