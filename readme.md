<div align="center">
    <img src="./assets/images/urai-logo-darkmode.png" height=300px>
    <h1>URAI Blog website</h1>
</div>

Welcome to the official Blog website of the [URAI
group](https://urai-group.com). In this repository, you will find the
source code of the website, all the blogs and related content.

---

## Developers guide

Code changes in this repository:

### 👉 Site Config

You can change the site title, base URL, language, theme, plugins, and
more from the `hugo.toml` file.

### 👉 Site Params

You can customize all the parameters from the
`config/_default/params.toml` file. This includes the logo, favicon,
search, SEO metadata, and more.

### 👉 Colors and Fonts

You can change the colors and fonts from the `data/theme.json` file.
This includes the primary color, secondary color, font family, and font
size.

### 👉 Social Links

You can change the social links from the `data/social.json` file. Add
your social links here, and they will automatically be displayed on the
site.

---

## 🛠 Advanced Usage

We have added some custom scripts to make your life easier. You can use
these scripts to help you with your development.

### 👉 Update Theme

If you want to update the theme, then you can use the following command.
It will update the theme to the latest version.

```bash
npm run update-theme
```

> **Note:** This command will work after running the `project-setup` script.

### 👉 Update Modules

We have added a lot of modules to this template. You can update all the
modules using the following command.

```bash
npm run update-modules
```

### 👉 Remove Dark Mode

If you want to remove dark mode from your project, you can use the
following command to remove dark mode from your project.

```bash
npm run remove-darkmode
```

> **Note:** This command will work before running the `project-setup`
> script. If you have already run the `project-setup` command, then you
> have to run `npm run theme-setup` first, and then you can run this
> command. Afterward, you can run `npm run project-setup` again.

### 👉 Remove Multilingual

If you want to remove multilingual from your project, you can use the
following command to remove multilingual from your project.

```bash
npm run remove-multilang
```

> **Note:** This command will work before running the `project-setup`
> script. If you have already run the `project-setup` command, then you
> have to run `npm run theme-setup` first, and then you can run this
> command. Afterward, you can run `npm run project-setup` again.

---

## 🚀 Build And Deploy

After you finish your development, you can build or deploy your project
almost everywhere. Let's see the process:

### 👉 Build Command

To build your project locally, you can use the following command.

```bash
npm run build
```

### 👉 Deployment

To deploy the website, just push your changes in this repository. The
[deployment workflow](./.github/workflows/hugo.yml) will take care of
the rest.

