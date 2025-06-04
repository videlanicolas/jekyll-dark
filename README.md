# jekyll-dark
A Jekyll dark theme for my website


## Theme Usage and Local Testing

This repository contains a custom Jekyll theme.

### Prerequisites

- Ruby and Bundler: Make sure you have Ruby and Bundler installed on your system. You can find installation instructions at [https://jekyllrb.com/docs/installation/](https://jekyllrb.com/docs/installation/).
- Jekyll: Install Jekyll gem: `gem install jekyll bundler`

### Running Locally

1.  **Clone the repository (if you haven't already):**
    ```bash
    git clone <repository_url>
    cd <repository_directory>
    ```
2.  **Install dependencies:**
    Navigate to the root directory of the theme and run:
    ```bash
    bundle install
    ```
    This command installs all the gems specified in the `Gemfile` (Jekyll will create/manage this).

3.  **Build and serve the site:**
    Use the following command to build the site and serve it locally:
    ```bash
    bundle exec jekyll serve --livereload
    ```
    - The site will typically be available at `http://127.0.0.1:4000/`.
    - The `--livereload` flag automatically refreshes the page in your browser when you make changes to the source files.

### Customization

-   **Configuration**: Edit `_config.yml` to change site title, author, social media links (GitHub, LinkedIn), description, etc.
-   **Styling**: Modify `assets/css/style.scss` to change the visual appearance (colors, fonts, layout). The theme uses SCSS for styling.
-   **Layouts**: Main layouts are in the `_layouts` directory (`default.html`, `post.html`, `project.html`).
-   **Includes**: Reusable components like header and footer are in `_includes`.
-   **Content**:
    -   **Homepage**: Edit `index.md` (or `index.markdown`).
    -   **Blog Posts**: Add markdown files to the `_posts` directory. Follow the naming convention `YYYY-MM-DD-your-post-title.md`.
    -   **Projects**: Add markdown files to the `_projects` directory. Update `projects.md` for the listing page if needed.

### Dark Theme

This theme is designed with a dark aesthetic. Key color variables and styles can be found in `assets/css/style.scss`.
