# hugo-notice
This is a simple theme component which provided a shortcode: `notice` to show notices. 

There are three types of notices: `tip`, `note`, `warning`. You can also add more types of notices if you want. Just modify the source file `layouts/shortcodes/notice.html` and the localization file `i18n/language.yaml`.

### Installation
You can just simply clone this project to your theme folder:
```shell
$ git clone https://github.com/Isoheptane/hugo-notice.git themes/hugo-notice
```
You can also add this repo as a submodule:
```shell
$ git submodule add https://github.com/Isoheptane/hugo-notice.git themes/hugo-notice
```
Then, add this theme component to your themes list.
Example with `config.yaml`:
```yaml
theme: ["hugo-notice", "others"]
```
### Usage
Use notice shortcode like this:
```go
{{< notice warning >}}
This is a warning message.
{{< /notice >}}
```
or like this:
```go
{{< notice note >}}
It's worth to notice that: ...
{{< /notice >}}
```

### Credits
This project is inspired by [`martignoni/hugo-notice`](https://github.com/martignoni/hugo-notice), a similar hugo notice module.
