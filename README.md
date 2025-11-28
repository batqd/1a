# Pomoc dydaktyczna dla programisty C++, Java JDK
[![.github/workflows/ci.yaml](https://github.com/pages-themes/hacker/actions/workflows/ci.yaml/badge.svg)](https://github.com/pages-themes/hacker/actions/workflows/ci.yaml) [![Gem Version](https://badge.fury.io/rb/jekyll-theme-hacker.svg)]( https://github.com/bartdurak/char)


*Jekyll theme  [zobacz projekt szablonu](http://pages-themes.github.io/hacker), or even [use it today](#usage).*
<img height="250" src="https://github.com/bartdurak/1a/blob/master/assets/images/batq_zdalne.png" width="250"/>

### [Strona główna](./index.md)
### [Git w CMD.exe windows ](./git_windows.md)
### [Skanowanie kalilinux](./Net_scan.md)
### [Zakładanie konta na github](./another-page.md)
## Strona zadeklarowana dla uczniów technikum "technik programista"
[Link do opisu](./another-page.html).
*Jekyll theme  [zobacz projekt szablonu](http://pages-themes.github.io/hacker), or even [use it today](#usage).*
### jesteś w pliku REDME.md a niżej umieściłem instrukcję założenia strony staycznej , jak ta.
[bartdurak.github.io/1a](https://bartdurak.github.io/1a/)
### 1. Przykład pliku README w popularnym obecnie jekyll

[Link do pełnego opisu strony](./another-page.html).

### 2. Opcjonalnie, jeśli chcesz wyświetlić podgląd swojej witryny na komputerze, dodaj następujące elementy do swojej witryny Gemfile: `Gemfile`:

    ```ruby
    gem "github-pages", group: :jekyll_plugins
    ```

## Personalizacja

### 2. Plik konfiguracji szablonu strony:

Secure  to motyw Jekylla dla GitHub Pages umieszczony w pliku `_config.yml`:

```yml
title: [Tytuł stony internetowej]
description: [krótki opis]
```

plik z kodem analizy odwiedzin strony

```yml
show_downloads: ["true" or "false" (unquoted) to indicate whether to provide a download URL]
google_analytics: [Your Google Analytics tracking ID]
```
### Arkusz stylów

Możesz dostosować kolorystykę strony, przez edycje pliku scss, więcej o tym na zajęciach
w 2 i 3 klasie.

1. Utwórz plik o nazwie `/assets/css/style.scss` w swojej witrynie 
2. Add the following content to the top of the file, exactly as shown:
    ```scss
    ---
    ---

    @import "{{ site.theme }}";
    ```
3. Dodaj dowolny niestandardowy CSS (lub Sass, w tym import), bezpośrednio po linii `@import` 

*Uwaga: jeśli chcesz zmienić zmienne Sass motywu, musisz ustawić nowe wartości przed linią `@import` w arkuszu stylów.*

### Praca z szablonem

1. W przypadku niektórych zmian, takich jak niestandardowy `favicon`, możesz dodać niestandardowe pliki do lokalnego folderu `_includes`. Pliki [dostarczone z motywem](https://github.com/pages-themes/hacker/tree/master/_includes) stanowią punkt wyjścia i są dołączone do [oryginalnego szablonu układu](https://github. com/pages-themes/hacker/blob/master/_layouts/default.html).
2. Aby uzyskać bardziej rozbudowane zmiany, [skopiuj oryginalny szablon](https://github.com/pages-themes/hacker/blob/master/_layouts/default.html) z repozytorium motywu<br />(*Pro- wskazówka: kliknij „raw”, aby ułatwić sobie kopiowanie*)
3. Create a file called `/_layouts/default.html` in your site
4. Paste the default layout content copied in the first step
5. Customize the layout as you'd like

###  Możesz dodać swoją stronę do usługi Google Analytics code. Dzięki temu będziesz widział statystyki twojej strony.

Google has released several iterations to their Google Analytics code over the years since this theme was first created. If you would like to take advantage of the latest code, paste it into `_includes/head-custom-google-analytics.html` in your Jekyll site.

### Zastępowanie adresów URL generowanych przez GitHub

Templates often rely on URLs supplied by GitHub such as links to your repository or links to download your project. If you'd like to override one or more default URLs:

1. Look at [the template source](https://github.com/pages-themes/hacker/blob/master/_layouts/default.html) to determine the name of the variable. It will be in the form of `{{ site.github.zip_url }}`.
2. Określ adres URL, którego szablon ma używać w pliku `_config.yml` Twojej witryny. Na przykład, jeśli zmienna to `site.github.url`, należy dodać:
    ```yml
    github:
      zip_url: http://example.com/download.zip
      another_url: another value
    ```
3. When your site is built, Jekyll will use the URL you specified, rather than the default one provided by GitHub.

*Note: You must remove the `site.` prefix, and each variable name (after the `github.`) should be indent with two space below `github:`.*

For more information, see [the Jekyll variables documentation](https://jekyllrb.com/docs/variables/).

## Mapa strony 

See the [open issues](https://github.com/pages-themes/hacker/issues) for a list of proposed features (and known issues).

## Projekt Secure 

The Secure theme is intended to make it quick and easy for GitHub Pages users to create their first (or 100th) website. The theme should meet the vast majority of users' needs out of the box, erring on the side of simplicity rather than flexibility, and provide users the opportunity to opt-in to additional complexity if they have specific needs or wish to further customize their experience (such as adding custom CSS or modifying the default layout). It should also look great, but that goes without saying.

### Krótka instrukcja pobrania i uruchomienia tego szablonu 

If you'd like to preview the theme locally (for example, in the process of proposing a change):

1. Clone down the theme's repository (`git clone https://github.com/pages-themes/hacker`)
2. `cd` into the theme's directory
3. Run `script/bootstrap` to install the necessary dependencies
4. Run `bundle exec jekyll serve` to start the preview server
5. Visit [`localhost:4000`](http://localhost:4000) in your browser to preview the theme

### Running tests

The theme contains a minimal test suite, to ensure a site with the theme would build successfully. To run the tests, simply run `script/cibuild`. You'll need to run `script/bootstrap` once before the test script will work.
````
