# Hugo Content

This is an example of a Hugo content module.

## Structure

```text
assets/
├── images/
│   ├── a.jpg
│   ├── b.jpg
│   └── c.jpg
└── videos/
    ├── a.mp4
    └── b.mp4
content/
└── articles/
    ├── article-1/
    │   ├── a.jpg
    │   └── index.md
    ├── article-2/
    │   ├── b.jpg
    │   └── index.md
    ├── article-3/
    │   ├── c.jpg
    │   └── index.md
    └── hugö.md
data/
└── fruit.json
```

## Usage

### To add this content to your Hugo project as a Hugo module

1. Initialize your project as a Hugo Module.

   ```bash
   hugo mod init foo/bar
   ```

2. Update your site configuration.

   ```toml
   [[module.imports]]
   path = "github.com/jmooring/hugo-content"
   ```

### To add this content to your Hugo project via npm

1. Install the package.

   ```bash
   npm install -D https://github.com/jmooring/hugo-content
   ```

2. Update your site configuration.

   ```toml
   [[module.mounts]]
   source = 'content'
   target = 'content'
 
   [[module.mounts]]
   source = 'node_modules/hugo-content/content'
   target = 'content'
   ```
  