# Hugo Module &ndash; Content

This is an example of a Hugo content module.

## Structure

```text
hugo-module-content/
├── assets/
│   ├── images/
│   │   ├── a.jpg
│   │   ├── b.jpg
│   │   └── c.jpg
│   └── videos/
│       ├── a.mp4
│       └── b.mp4
├── content/
│   └── articles/
│       ├── article-1/
│       │   ├── a.jpg
│       │   └── index.md
│       ├── article-2/
│       │   ├── b.jpg
│       │   └── index.md
│       └── article-3/
│           ├── c.jpg
│           └── index.md
├── data/
│   └── fruit.json
└── config.toml
```

## Configuration

To add this module to your project, initialize your project as a Hugo module:

```text
hugo mod init foo
```

In the above, `foo` is typically something like `github.com/user/project`.

Then add this to your site configuration:

```text
[[module.imports]]
path = 'github.com/jmooring/hugo-module-content'
```
