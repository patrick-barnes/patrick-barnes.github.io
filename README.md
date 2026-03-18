# patrick-barnes.github.io

My portolio website.

- CNAME: https://pjbarnes.dev
- Points to: https://patrick-barnes.github.io/
- Repo: https://github.com/patrick-barnes/patrick-barnes.github.io

## Tech stack

Powered by:

- Ruby 3.x
- bundler (gem management)
- Jekyll (Ruby gem for static websites)

Why? Because Jekyll is the only tech that
seamlessly integrates with github pages without
requiring custom actions.

## Local setup

1. Install [RubyInstaller+Devkit 3.x](https://rubyinstaller.org/downloads/) with default options.

2. `ruby -v` - to verify ruby version

3. `gem install bundler` - for gem management

4. `bundle install` - dependencies from `Gemfile`

5. `bundle exec jekyll serve --livereload --incremental`

6. Local preview: http://127.0.0.1:4000/

If things get weird, clear the cache:

`bundle exec jekyll clean`

## Publishing

Commit and push changes.

Preview the [build](https://github.com/patrick-barnes/patrick-barnes.github.io/actions).

Access the live site: https://pjbarnes.dev/
