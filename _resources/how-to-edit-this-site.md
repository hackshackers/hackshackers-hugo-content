---
title: How to edit this site
url: resources/how-to-edit-this-site
---

Not only is the code for this site open source, the content is too. Anyone in the Hacks/Hackers community can propose a new post or suggest edits to an existing one by opening a pull request on GitHub. All you need is a GitHub account.

## Creating a post

Fork [hackshackers-hugo-content][1] (there's a button in the top right corner).

In your new repository, click the "Create new file" button. (see below re: [directories and URLs](#note-directories-and-urls) Next you'll see GitHub's text editor, which lets you write and preview [Markdown][3].

When you're ready, click "Create new file". (It's safe to commit directly to the `master` branch within your own fork.)

Then go back to the root of your fork of the repository, and click "New pull request".

(jump to [Your Pull Request](#your-pull-request))

## Editing a post

Individual pages like this one have a big link labeled "Suggest Edits" below the page title. Click it! GitHub will prompt you to fork the repository and propose changes. Or you can browse the repository to find the page you want to edit, then click this link:

![Edit a page in GitHub](/content-images/resources/edit-page.png)

Make your edits and click "Propose file change".

## Your Pull Request

You'll see a dialog like this to review your changes and confirm that you really do want to create a pull request.

![Create pull request dialog](/content-images/resources/create-pr.png)

Click "Create pull request" and proceeed to the next screen. You can give your PR a title and description before making it official.

Now, one of the site editors can review your proposed changes and merge them back into the original repository. Keep an eye out for email notifications from GitHub regarding your PR.

#### Note: directories and URLs

[Hugo][2] determines the post's URL (by default) using the location of the source Markdown file. So if you're writing a blog post in July 2017, your file `blog/2017/07/my-post.md` would become `http://hackshackers.com/blog/2017/07/my-post/`

Conveniently, GitHub's text editor lets you place your new file in whatever directory you want by typing a `/`:

![Creating a new directory](/content-images/resources/new-directory.png)

#### Note: embedding images

Once you have forked the repo, you can add images directly through GitHub using the "Upload files" button. Importantly, you have to navigate to the directory where you want the files _before_ you upload them. In our case, that is somewhere inside the `content-images` directory.

To embed the image in an article, you would then do something like:

```
![Img alt text](/content-images/path/to/my/image.jpg)
```

[1]: https://github.com/hackshackers/hackshackers-hugo-content
[2]: https://gohugo.io
[3]: https://guides.github.com/features/mastering-markdown/