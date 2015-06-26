# ox-jekyll-subtree 

Extension to ox-jexkyll for better export of subtrees. This is only
possible thanks to `ox-jekyll`, from the
[org-octopress](https://github.com/yoshinari-nomura/org-octopress)
repo (a copy is provided in this repo).

*Please note, this is not a package, this is a script. Feel free to
 submit issues if you run into problems, just be aware that this does
 not fully conform with usual package standards.*

## Usage

Place this in your `load-path`, add the following lines to your init file, and invoke `M-x endless/export-to-blog` to export a subtree as a blog post.

```
(autoload 'endless/export-to-blog "jekyll-once")
(setq org-jekyll-use-src-plugin t)

;; Obviously, these two need to be changed for your blog.
(setq endless/blog-base-url "http://endlessparentheses.com/")
(setq endless/blog-dir (expand-file-name "~/Git-Projects/blog/"))
```
