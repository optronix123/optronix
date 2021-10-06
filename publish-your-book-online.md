# Publish your book online

Once you’ve built the HTML for your book, you can host it online. The best way to do this is with a service that hosts **static websites** \(because that’s what you have just created with Jupyter Book\). In this tutorial, we’ll cover how to publish your book online with GitHub Pages, a popular and free online hosting platform.

### Create an online repository for your book[¶](https://jupyterbook.org/start/publish.html#create-an-online-repository-for-your-book)

In order to connect your hosted book with your book’s source content, you should put your book’s source content in a public repository. This section describes one approach to create your own GitHub repository and add your book’s content to it.

1. First, log in to GitHub, then go to the “create a new repository” page: [https://github.com/new](https://github.com/new)
2. Next, give your online repository a name and a description. Make your repository public and do not initialize it with a README file, then click “Create repository”.
3. Now, clone the \(currently empty\) online repository to a location on your local computer. You can do this via the command line with:

   ```text
   git clone https://github.com/<my-org>/<my-repository-name>
   ```

Copy all of your book files and folders into this newly cloned repository. For example, if you created your book locally with `jupyter-book create mylocalbook` and your new repository is called `myonlinebook`, you could do this via the command line with:

```text
cp -r mylocalbook/* myonlinebook/
```

Now you need to sync your local and remote \(i.e., online\) repositories. You can do this with the following commands:

