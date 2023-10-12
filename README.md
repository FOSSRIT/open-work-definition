# Open Work Definition
Built with Jekyll, Tailwind, and :heart:

## Development & Deployment

Install Jekyll on your system, or from the local repository.  On Linux, the latter can be accomplished using the commands

```bash
bundle install
```

A local webserver can now be created using the command

```bash
bundle exec jekyll serve
```

Or if you're using a system-wide Jekyll install, such as one from a package repo, run just

```bash
jekyll serve
```

A build for deployment can be created using

```
jekyll build

# or

bundle exec jekyll build
```

### Pushing With GitHub Actions
You may run into this GitHub actions error when deploying the site
`
Error: The process '/opt/hostedtoolcache/Ruby/[RUBY_VERSION]/x64/bin/bundle' failed with exit code 16
`.
It can be fixed by adding Linux support to your Gemfile by locally running
`
bundle lock --add-platform x86_64-linux
`.

--------------------
:art: Website design :art: by Daechan Kim & Matthew Incardona.
