# Plain Vanilla GitHub Pages README
The purpose of this project is to make as easy as possible for less-technical people to create and host basic web pages for free on [GitHub Pages](https://pages.github.com/).

[Check out my YouTube video on how to get started using this template](https://youtu.be/jlkHEmgQhGU)

## Getting started

### Copying the template and setting up publishing
1. Press the `Use this template` button on the `Code` tab.
1. Go to the `Settings` tab and then go to the `Pages` settings.
1. Set the `Source` to `main` and press `Save`.

You'll see a URL show up, but the site takes a few minutes before it's actually live. In the meantime, try creating a page.

### Creating your first page
1. Go to the `Code` tab.
1. Press the `Add File` button and select `Create new file`.
1. Name the page, for example, `first-page.md`. (Note the lack of spaces and the inclusion of the .md extension.)
1. Add a title in the front matter:
    ```
    ---
    title: First Page
    ---
    ```
1. Add some content using [markdown](https://guides.github.com/features/mastering-markdown/) syntax. For example, you could start with a heading and paragraph like this:
    ```
    # First page
    This is my first page.
    ```
5. Scroll down to the bottom of the page and press `Commit new file`.

### Checking your page online
1. On the Code tab, find and press the `Environments` link. (It may be in the right column.)
1. On the next page (Deployments), press the `View deployment` button. (You should see the default homepage load.)
1. In the address bar of the browser, add the name of your page _using the HTML extension_ and press return. For example: `first-page.html`. (The full address will be something like this: `https://pglevy.github.io/plain-vanilla-gh-pages/first-page.html`)

You should see the new page you created.

## Next steps
Now that you know how to create pages, here are some other things you can do:
- Create more pages.
- Update `index.md` (the homepage) with your own content.
- Add links between pages so it works like a website.
- Copy component code snippets from the [Pico CSS Framework](https://picocss.com/docs) to add more advanced functionality to your pages.
- Customize your site language, title, and description in the `metadata.yml` file located in the `_data` folder.

## Default `body` and `main` styling classes
- There are no classes on the `body` element by default.
- The `main` element includes the `container` class. This sets a maximum width for the content area.
- To override these, add these settings to the front matter of your content page: `body-style` and `main-style`.

For example:
```
title: Home
main-style: container-fluid
```

If you want to replace the default with nothing, do this:
```
title: My Page
main-style: ""
```

## Mixing HTML elements and Markdown in your .md pages
To use markdown inside of traditional HTML elements, add `markdown="1"` as a parameter to the HTML element. For example:

```
<section markdown="1">
  ![Screenshot of "create a new repository" action](assets/img/create-repo.jpg)
</section>
```

## Working with local CSS
By default, the site will load the Pico CSS from a hosted site (CDN). If you're working offline or don't have access to this for some reason, you can use a copy of the CSS file included in the repo. In `_config.yml`, change `useLocalCss` to `true`.

```
useLocalCss: true
```

## Work with site preview using the GitHub Codespaces remote dev environment
This project is configured to work with Codespaces. This allows you work on variations of the site in a remote dev environment in your browser so you can try things out without publishing directly to the live, `main` branch.

To use this option, select `Open in a codespace` from the `Use this template` menu button.

For more information, see the [GitHub documentation](https://docs.github.com/en/codespaces/developing-in-codespaces/creating-a-codespace-from-a-template#creating-a-codespace-from-a-template-repository).

## What to do if you're having problems
- Try starting over with a new repository and follow the instructions again.
- If it's still not working, [create an issue in the original Plain Vanilla GitHub Pages repo](https://github.com/lowcodelounge/plain-vanilla-gh-pages/issues), and I'll try to help.

## Credit and license
This project was created using the [GitHub Pages gem for Jekyll](https://github.com/github/pages-gem). It is licensed under [The Unlicense](https://github.com/pglevy/plain-vanilla-gh-pages/blob/main/LICENSE), which allows everything and promises nothing. 😎

Favicon is `Soft Ice Cream` from [Twemoji](https://twemoji.twitter.com/), licensed under [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/).
