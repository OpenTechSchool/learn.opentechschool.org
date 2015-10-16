# OpenTechSchool Materials Landing

A simple one-page landing for all of OTS' workshop materials.

Built using the [Gumby Framework](http://gumbyframework.com).
And jekyll, and compass.

You can edit / add workshops simply by editing the yaml
`sections` dictionary found in `_config.yml`.

To build this site, you'll need Ruby installed, and possibly Node.js.

### Ruby

Use `bundle install`, or install the `compass`, `jekyll` and
`modular-scale` gems.

To run the site, use `compass watch` in one terminal and `jekyll serve -w` in
another, then visit http://localhost:4000/

CSS adjustments are made in `sass/_custom.scss` and `sass/_fonts.scss`.

Jekyll might not automatically rebuild the site if you have changed
`_config.yml`, so I just `rm -r _site/*` before restarting the server again.

### Node.js

Only needed to update gumby.

Node requirements: `bower`, `claymate`. These two are designed to be installed
globally (`[sudo ]npm install -g bower claymate`).

To update gumby, use `bower update gumby`. To then rebuild it, use
`claymate build`.
