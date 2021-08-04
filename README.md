<p align="center">
    <h1 align="center">Blog</h1>
    <p align="center">
      <img src="https://github.com/junnei/blog/blob/main/assets/images/logo.gif?raw=true">
    </p>
    <p align="center">
        A collection of contents studied by myself.
    </p>
    <h3>
        <p align="center">
            <strong>
                <a href="https://junnei.github.io/blog/en">Go to Project Page!</a>
            </strong>
        </p>
    </h3>
    <br>
    <p align="center">
        <a href="http://creativecommons.org/licenses/by-nc-sa/4.0/" alt="CC BY-NC-SA 4.0">
            <img src="https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-blue.svg">
        </a>
    </p>
    <br><br>
</p>



## Contributors

All of them contributed in this project with <b>high-quality contents!</b>

<b>Thanks goes to these wonderful people :</b>

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore -->
| [<img src="https://avatars.githubusercontent.com/u/41983244?v=4" width="128px;"/><br><b>Seongjun Jang</b>](https://github.com/junnei)<br><br><a href="https://junnei.github.io"><img src="https://edent.github.io/SuperTinyIcons/images/svg/github.svg" width="24" title="GitHub" /></a> <a href="https://www.linkedin.com/in/xun"><img src="https://edent.github.io/SuperTinyIcons/images/svg/linkedin.svg" width="24" title="LinkedIn" /></a> <a href="https://www.instagram.com/worg._.grow"><img src="https://edent.github.io/SuperTinyIcons/images/svg/instagram.svg" width="24" title="Instagram" /></a> <a href="https://soundcloud.com/ljobavastjqn"><img src="https://edent.github.io/SuperTinyIcons/images/svg/soundcloud.svg" width="24" title="SoundCloud" /></a>| Waiting for contribute |
| :---: | :---: | 
<!-- ALL-CONTRIBUTORS-LIST:END -->

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/junnei/blog.

Feel free to make issues!

Feel free to contribute with high-quality contents!


### Requirements

*(If Docker, just run it and Open your browser at [`http://localhost:4000`](http://localhost:4000))*
```bash
    $ docker-compose up
```

First, we need to install ruby (v2.7.3 in my case)
```bash
## Linux
$ sudo apt install ruby ruby-dev build-essential

## MacOS
$ brew install ruby
```

And then install `jekyll` :

```bash
$ gem install bundler jekyll
```

### Installation

First, fork this repository to your local machine.

```bash
$ git fork https://github.com/junnei/blog
$ cd mml
```


Install gem dependencies by :

```bash
$ bundle install
```

You should preview the site contents before contributing, so just run it by:

```bash
$ bundle exec jekyll serve
```
This starts a Jekyll server, and now you could test whatever you added.

Open your browser at [`http://localhost:4000`](http://localhost:4000)

### Submitting code changes:

Add your information in `_data/contributors.yml`.

```yml
#ex)
junnei:
  kr:
    name: 장성준
  en:
    name: Seongjun Jang
[YOUR_GITHUB_ID]:
  kr:
    name: [YOUR_NAME/KR](홍길동)
  en:
    name: [YOUR_NAME/EN](John Doe)c
```

- Open a [Pull Request](https://github.com/junnei/blog/pulls)
- Await code review
- Ta-da! You've become a contributor!😆

### Progress of Studying

| Progress  | Contents  | Assigned to   | Update Date | Current Status | 
|-----------|-----------|---------------|-------------|----------------|
|  | Music-001    |[Seongjun Jang(장성준)](https://github.com/junnei)| 2021-08-01 | ✔️


## License

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
