# Jekyll Setup & Theme Migration History
Date: 2025-12-07

## 1. Initial Setup
- **Objective**: Initialize a GitHub Pages compatible Jekyll site.
- **Action**: Used `github-pages` gem.
- **Result**: Basic Jekyll site created with default Minima theme.

## 2. Theme Migration (Minimal Mistakes)
- **Objective**: Switch to a theme suitable for photography and AI image portfolio.
- **Theme Chosen**: [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/)
- **Installation Method**: `remote_theme` (Best practice for GitHub Pages).
    - **Gemfile**: Added `gem "jekyll-remote-theme"` and `gem "jekyll-include-cache"`.
    - **_config.yml**: set `remote_theme: "mmistakes/minimal-mistakes"`.

## 3. Configuration
- **Skin**: Set to `dark` (`minimal_mistakes_skin: "dark"`).
- **Plugins**: Enabled `jekyll-feed`, `jekyll-remote-theme`, `jekyll-include-cache`.
- **Site Details**: Updated title to "Compassute" and URL to `https://compassute.github.io`.

## 4. Layout Updates
To match Minimal Mistakes requirements:
- **`index.md`**:
    - Layout changed to `home`.
    - Added `author_profile: true`.
- **`about.md`**:
    - Layout changed to `single`.
- **`_posts/`**:
    - Default post layout changed from `post` to `single` to avoid build warnings.

## 5. How to Run
```bash
bundle install
bundle exec jekyll serve
```
