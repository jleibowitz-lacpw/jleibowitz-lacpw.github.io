# jleibowitz-lacpw.github.io

Personal GitHub Pages site (Jekyll) experimenting with a lightweight digital garden and simple navigation.

## Quick Preview in Codespaces

1. Open this repo on GitHub. Click the green Code button -> "Create codespace on main".
2. Wait for the devcontainer to finish (it will run `bundle install`).
3. Start the Jekyll server:
	```bash
	bundle exec jekyll serve --livereload --host 0.0.0.0
	```
4. Use the forwarded port (4000) to view the site.

## Local Preview with Docker (alternative)
```powershell
docker run --rm -it -p 4000:4000 -v "${PWD}:/srv/jekyll" -w /srv/jekyll ghcr.io/actions/jekyll-build-pages:v1.0.13 jekyll serve --host 0.0.0.0 --livereload --force_polling
```

## Structure
```
_config.yml        # Site metadata & plugins
_layouts/page.html # Layout with header/footer includes
_includes/         # Reusable fragments (header, footer)
style.css          # Custom styles (later could move to assets/css)
Gemfile            # GitHub Pages gem dependencies
.devcontainer/     # Codespaces environment config
```

## License
See `LICENSE` file. Content reflects personal views only.

---
"The postings on this website are my own and do not represent the views or opinions of my employer."
