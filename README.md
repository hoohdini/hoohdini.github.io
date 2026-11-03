# HOOHDINI 블로그

Jekyll + [Chirpy](https://github.com/cotes2020/jekyll-theme-chirpy) 테마. `main`에 push하면 GitHub Actions가 GitHub Pages로 배포합니다.

## 글쓰기 (브라우저에서)

1. https://hoohdini.github.io/admin/ 에 들어갑니다.
2. **Sign In Using Access Token**을 누르고 GitHub 토큰을 붙여넣습니다. (토큰 만드는 법은 아래)
3. **글 → 새 글**에서 제목·카테고리·태그를 채우고 본문을 씁니다. 이미지는 본문에 붙여넣거나 끌어다 놓으면 `assets/img/posts/`에 올라갑니다.
4. **저장**을 누르면 `main`에 커밋되고, 1~2분 뒤 사이트에 반영됩니다.

- 수식(`$...$`)이 들어간 글은 본문 툴바에서 **Markdown 모드**로 바꿔서 편집하세요. 서식 모드는 수식 기호를 이스케이프할 수 있습니다.
- 임시 저장만 하고 싶으면 **공개**를 끄고 저장합니다(`published: false`).

### 토큰 만들기 (한 번만)

GitHub → Settings → Developer settings → Personal access tokens → **Fine-grained tokens** → Generate new token

- Repository access: **Only select repositories** → `hoohdini.github.io`
- Permissions → Repository permissions → **Contents: Read and write**
- 만료일은 원하는 대로(예: 1년). 토큰은 이 브라우저에만 저장됩니다. 공용 PC에서는 쓰지 마세요.

---

# Chirpy Starter

[![Gem Version](https://img.shields.io/gem/v/jekyll-theme-chirpy)][gem]&nbsp;
[![GitHub license](https://img.shields.io/github/license/cotes2020/chirpy-starter.svg?color=blue)][mit]

When installing the [**Chirpy**][chirpy] theme through [RubyGems.org][gem], Jekyll can only read files in the folders
`_data`, `_layouts`, `_includes`, `_sass` and `assets`, as well as a small part of options of the `_config.yml` file
from the theme's gem. If you have ever installed this theme gem, you can use the command
`bundle info --path jekyll-theme-chirpy` to locate these files.

The Jekyll team claims that this is to leave the ball in the user’s court, but this also results in users not being
able to enjoy the out-of-the-box experience when using feature-rich themes.

To fully use all the features of **Chirpy**, you need to copy the other critical files from the theme's gem to your
Jekyll site. The following is a list of targets:

```shell
.
├── _config.yml
├── _plugins
├── _tabs
└── index.html
```

To save you time, and also in case you lose some files while copying, we extract those files/configurations of the
latest version of the **Chirpy** theme and the [CD][CD] workflow to here, so that you can start writing in minutes.

## Usage

Check out the [theme's docs](https://github.com/cotes2020/jekyll-theme-chirpy/wiki).

## Contributing

This repository is automatically updated with new releases from the theme repository. If you encounter any issues or want to contribute to its improvement, please visit the [theme repository][chirpy] to provide feedback.

## License

This work is published under [MIT][mit] License.

[gem]: https://rubygems.org/gems/jekyll-theme-chirpy
[chirpy]: https://github.com/cotes2020/jekyll-theme-chirpy/
[CD]: https://en.wikipedia.org/wiki/Continuous_deployment
[mit]: https://github.com/cotes2020/chirpy-starter/blob/master/LICENSE
