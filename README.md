<p align="center">
 <img width="100px" src="https://res.cloudinary.com/anuraghazra/image/upload/v1594908242/logo_ccswme.svg" align="center" alt="GitHub Readme Stats" />
 <h2 align="center">Nova Github Profile</h2>
 <p align="center">Developer of Nova Bot and Nova Documentation</p>
</p>

> [!NOTE]\
> This is the only Nova official Github Profile.

#### All inbuilt themes

**Nova** is the all-in-one solution your Discord server needs. With a powerful suite of features, it covers everything from **Moderation** to **Economy** and even **Suggestion** management. Whether you're looking for a seamless server experience or just some good old fun, **Nova** has got you covered. 

### Customization

You can customize the appearance of all your cards however you wish with URL parameters.

#### Common Options

*   `title_color` - Card's title color *(hex color)*. Default: `2f80ed`.
*   `text_color` - Body text color *(hex color)*. Default: `434d58`.
*   `icon_color` - Icons color if available *(hex color)*. Default: `4c71f2`.
*   `border_color` - Card's border color *(hex color)*. Default: `e4e2e2` (Does not apply when `hide_border` is enabled).
*   `bg_color` - Card's background color *(hex color)* **or** a gradient in the form of *angle,start,end*. Default: `fffefe`
*   `hide_border` - Hides the card's border *(boolean)*. Default: `false`
*   `theme` - Name of the theme, choose from [all available themes](./themes/README.md). Default: `default` theme.
*   `cache_seconds` - Sets the cache header manually *(min: 14400, max: 86400)*. Default: `14400 seconds (4 hours)`.
*   `locale` - Sets the language in the card *(e.g. cn, de, es, etc.)*. Default: `en`.
*   `border_radius` - Corner rounding on the card. Default: `4.5`.

> [!WARNING]\
> We use caching to decrease the load on our servers (see <https://github.com/anuraghazra/github-readme-stats/issues/1471#issuecomment-1271551425>). Our cards have a default cache of 4 hours (14400 seconds). Also, note that the cache is clamped to a minimum of 4 hours and a maximum of 24 hours.

##### Gradient in bg\_color

You can provide multiple comma-separated values in the bg\_color option to render a gradient with the following format:

    &bg_color=DEG,COLOR1,COLOR2,COLOR3...COLOR10

#### Stats Card Exclusive Options

*   `hide` - Hides the [specified items](#hiding-individual-stats) from stats *(Comma-separated values)*. Default: `[] (blank array)`.
*   `hide_title` - *(boolean)*. Default: `false`.
*   `card_width` - Sets the card's width manually *(number)*. Default: `500px  (approx.)`.
*   `hide_rank` - *(boolean)* hides the rank and automatically resizes the card width. Default: `false`.
*   `rank_icon` - Shows alternative rank icon (i.e. `github`, `percentile` or `default`). Default: `default`.
*   `show_icons` - *(boolean)*. Default: `false`.
*   `include_all_commits` - Counts total commits instead of just the current year commits *(boolean)*. Default: `false`.
*   `line_height` - Sets the line height between text *(number)*. Default: `25`.
*   `exclude_repo` - Excludes stars from specified repositories *(Comma-separated values)*. Default: `[] (blank array)`.
*   `custom_title` - Sets a custom title for the card. Default:  `<username> GitHub Stats`.
*   `text_bold` - Uses bold text *(boolean)*. Default: `true`.
*   `disable_animations` - Disables all animations in the card *(boolean)*. Default: `false`.
*   `ring_color` - Color of the rank circle *(hex color)*. Defaults to the theme ring color if it exists and otherwise the title color.
*   `number_format` - Switches between two available formats for displaying the card values `short` (i.e. `6.6k`) and `long` (i.e. `6626`). Default: `short`.
*   `show` - Shows [additional items](#showing-additional-individual-stats) on stats card (i.e. `reviews`, `discussions_started`, `discussions_answered`, `prs_merged` or `prs_merged_percentage`) *(Comma-separated values)*. Default: `[] (blank array)`.

> [!NOTE]\
> When hide\_rank=`true`, the minimum card width is 270 px + the title length and padding.

#### Repo Card Exclusive Options

*   `show_owner` - Shows the repo's owner name *(boolean)*. Default: `false`.

#### Gist Card Exclusive Options

*   `show_owner` - Shows the gist's owner name *(boolean)*. Default: `false`.

#### Language Card Exclusive Options

*   `hide` - Hides the languages specified from the card *(Comma-separated values)*. Default: `[] (blank array)`.
*   `hide_title` - *(boolean)*. Default: `false`.
*   `layout` - Switches between five available layouts `normal` & `compact` & `donut` & `donut-vertical` & `pie`. Default: `normal`.
*   `card_width` - Sets the card's width manually *(number)*. Default `300`.
*   `langs_count` - Shows more languages on the card, between 1-20 *(number)*. Default: `5` for `normal` and `donut`, `6` for other layouts.
*   `exclude_repo` - Excludes specified repositories *(Comma-separated values)*. Default: `[] (blank array)`.
*   `custom_title` - Sets a custom title for the card *(string)*. Default `Most Used Languages`.
*   `disable_animations` - Disables all animations in the card *(boolean)*. Default: `false`.
*   `hide_progress` - Uses the compact layout option, hides percentages, and removes the bars. Default: `false`.
*   `size_weight` - Configures language stats algorithm *(number)* (see [Language stats algorithm](#Language-stats-algorithm)), defaults to 1.
*   `count_weight` - Configures language stats algorithm *(number)* (see [Language stats algorithm](#Language-stats-algorithm)), defaults to 0.

> [!WARNING]\
> Language names should be URI-escaped, as specified in [Percent Encoding](https://en.wikipedia.org/wiki/Percent-encoding)
> (i.e: `c++` should become `c%2B%2B`, `jupyter notebook` should become `jupyter%20notebook`, etc.) You can use
> [urlencoder.org](https://www.urlencoder.org/) to help you do this automatically.

#### Wakatime Card Exclusive Options

*   `hide` - Hides the languages specified from the card *(Comma-separated values)*. Default: `[] (blank array)`.
*   `hide_title` - *(boolean)*. Default `false`.
*   `line_height` - Sets the line height between text *(number)*. Default `25`.
*   `hide_progress` - Hides the progress bar and percentage *(boolean)*. Default `false`.
*   `custom_title` - Sets a custom title for the card *(string)*. Default `Wakatime Stats`.
*   `layout` - Switches between two available layouts `default` & `compact`.  Default `default`.
*   `langs_count` - Limits the number of languages on the card, defaults to all reported languages *(number)*.
*   `api_domain` - Sets a custom API domain for the card, e.g. to use services like [Hakatime](https://github.com/mujx/hakatime) or [Wakapi](https://github.com/muety/wakapi) *(string)*. Default `Waka API`.

***

# GitHub Extra Pins

GitHub extra pins allow you to pin more than 6 repositories in your profile using a GitHub readme profile.

Yay! You are no longer limited to 6 pinned repositories.

### Usage

Copy-paste this code into your readme and change the links.

Endpoint: `api/pin?username=anuraghazra&repo=github-readme-stats`

```md
[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=anuraghazra&repo=github-readme-stats)](https://github.com/anuraghazra/github-readme-stats)
```

### Demo

![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=anuraghazra\&repo=github-readme-stats)

Use [show\_owner](#repo-card-exclusive-options) query option to include the repo's owner username

![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=anuraghazra\&repo=github-readme-stats\&show_owner=true)

# GitHub Gist Pins

GitHub gist pins allow you to pin gists in your GitHub profile using a GitHub readme profile.

### Usage

Copy-paste this code into your readme and change the links.

Endpoint: `api/gist?id=bbfce31e0217a3689c8d961a356cb10d`

```md
[![Gist Card](https://github-readme-stats.vercel.app/api/gist?id=bbfce31e0217a3689c8d961a356cb10d)](https://gist.github.com/Yizack/bbfce31e0217a3689c8d961a356cb10d/)
```

### Demo

![Gist Card](https://github-readme-stats.vercel.app/api/gist?id=bbfce31e0217a3689c8d961a356cb10d)

Use [show\_owner](#gist-card-exclusive-options) query option to include the gist's owner username

![Gist Card](https://github-readme-stats.vercel.app/api/gist?id=bbfce31e0217a3689c8d961a356cb10d\&show_owner=true)

# Top Languages Card

The top languages card shows a GitHub user's most frequently used languages.

> [!WARNING]\
> By default, the language card shows language results only from public repositories. To include languages used in private repositories, you should [deploy your own instance](#deploy-on-your-own) using your own GitHub API token.

> [!NOTE]\
> Top Languages does not indicate the user's skill level or anything like that; it's a GitHub metric to determine which languages have the most code on GitHub. It is a new feature of github-readme-stats.

> [!WARNING]\
> This card shows languages usage only inside your own non-forked repositories, not depending from who is the author of the commits. It does not include your contributions into another users/organizations repositories. Currently there are no way to get this data from GitHub API. If you want this behavior to be improved you can support [this feature request](https://github.com/orgs/community/discussions/18230) created by [@rickstaa](https://github.com/rickstaa) inside GitHub Community.

> [!WARNING]\
> Currently this card shows data only about first 100 repositories. This is because GitHub API limitations which cause downtimes of public instance (see [#1471](https://github.com/anuraghazra/github-readme-stats/issues/1471)). In future this behavior will be improved by releasing GitHub action or providing environment variable for user's own instances.

### Usage

Copy-paste this code into your readme and change the links.

Endpoint: `api/top-langs?username=anuraghazra`

```md
[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra)](https://github.com/anuraghazra/github-readme-stats)
```

### Language stats algorithm

We use the following algorithm to calculate the languages percentages on the language card:

```js
ranking_index = (byte_count ^ size_weight) * (repo_count ^ count_weight)
```

By default, only the byte count is used for determining the languages percentages shown on the language card (i.e. `size_weight=1` and `count_weight=0`). You can, however, use the `&size_weight=` and `&count_weight=` options to weight the language usage calculation. The values must be positive real numbers. [More details about the algorithm can be found here](https://github.com/anuraghazra/github-readme-stats/issues/1600#issuecomment-1046056305).

*   `&size_weight=1&count_weight=0` - *(default)* Orders by byte count.
*   `&size_weight=0.5&count_weight=0.5` - *(recommended)* Uses both byte and repo count for ranking
*   `&size_weight=0&count_weight=1` - Orders by repo count

```md
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra&size_weight=0.5&count_weight=0.5)
```

### Exclude individual repositories

You can use the `&exclude_repo=repo1,repo2` parameter to exclude individual repositories.

```md
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra&exclude_repo=github-readme-stats,anuraghazra.github.io)
```

### Hide individual languages

You can use `&hide=language1,language2` parameter to hide individual languages.

```md
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra&hide=javascript,html)
```

### Show more languages

You can use the `&langs_count=` option to increase or decrease the number of languages shown on the card. Valid values are integers between 1 and 20 (inclusive). By default it was set to `5` for `normal` & `donut` and `6` for other layouts.

```md
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra&langs_count=8)
```

### Compact Language Card Layout

You can use the `&layout=compact` option to change the card design.

```md
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra&layout=compact)
```

### Donut Chart Language Card Layout

You can use the `&layout=donut` option to change the card design.

```md
[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra&layout=donut)](https://github.com/anuraghazra/github-readme-stats)
```

### Donut Vertical Chart Language Card Layout

You can use the `&layout=donut-vertical` option to change the card design.

```md
[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra&layout=donut-vertical)](https://github.com/anuraghazra/github-readme-stats)
```

### Pie Chart Language Card Layout

You can use the `&layout=pie` option to change the card design.

```md
[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra&layout=pie)](https://github.com/anuraghazra/github-readme-stats)
```

### Hide Progress Bars

You can use the `&hide_progress=true` option to hide the percentages and the progress bars (layout will be automatically set to `compact`).

```md
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra&hide_progress=true)
```

### Demo

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra)

*   Compact layout

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra\&layout=compact)

*   Donut Chart layout

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra\&layout=donut)](https://github.com/anuraghazra/github-readme-stats)

*   Donut Vertical Chart layout

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra\&layout=donut-vertical)](https://github.com/anuraghazra/github-readme-stats)

*   Pie Chart layout

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra\&layout=pie)](https://github.com/anuraghazra/github-readme-stats)

*   Hidden progress bars

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra\&hide_progress=true)

# Wakatime Stats Card

> [!WARNING]\
> Please be aware that we currently only show data from Wakatime profiles that are public. You therefore have to make sure that **BOTH** `Display code time publicly` and `Display languages, editors, os, categories publicly` are enabled.

Change the `?username=` value to your [Wakatime](https://wakatime.com) username.

```md
[![Harlok's wakatime stats](https://github-readme-stats.vercel.app/api/wakatime?username=ffflabs)](https://github.com/anuraghazra/github-readme-stats)
```

### Demo

![Harlok's wakatime stats](https://github-readme-stats.vercel.app/api/wakatime?username=ffflabs)

![Harlok's wakatime stats](https://github-readme-stats.vercel.app/api/wakatime?username=ffflabs\&hide_progress=true)

*   Compact layout

![Harlok's wakatime stats](https://github-readme-stats.vercel.app/api/wakatime?username=ffflabs\&layout=compact)

***

# All Demos

*   Default

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra)

*   Hiding specific stats

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra\&hide=contribs,issues)

*   Showing additional stats

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra\&show_icons=true\&show=reviews,discussions_started,discussions_answered,prs_merged,prs_merged_percentage)

*   Showing icons

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra\&hide=issues\&show_icons=true)

*   Shows Github logo instead rank level

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra\&rank_icon=github)

*   Shows user rank percentile instead of rank level

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra\&rank_icon=percentile)

*   Customize Border Color

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra\&border_color=2e4058)

*   Include All Commits

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra\&include_all_commits=true)

*   Themes

Choose from any of the [default themes](#themes)

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra\&show_icons=true\&theme=radical)

*   Gradient

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra\&bg_color=30,e96443,904e95\&title_color=fff\&text_color=fff)

*   Customizing stats card

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api/?username=anuraghazra\&show_icons=true\&title_color=fff\&icon_color=79ff97\&text_color=9f9f9f\&bg_color=151515)

*   Setting card locale

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api/?username=anuraghazra\&locale=es)

*   Customizing repo card

![Customized Card](https://github-readme-stats.vercel.app/api/pin?username=anuraghazra\&repo=github-readme-stats\&title_color=fff\&icon_color=f9f9f9\&text_color=9f9f9f\&bg_color=151515)

*   Gist card

![Gist Card](https://github-readme-stats.vercel.app/api/gist?id=bbfce31e0217a3689c8d961a356cb10d)

*   Customizing gist card

![Gist Card](https://github-readme-stats.vercel.app/api/gist?id=bbfce31e0217a3689c8d961a356cb10d&theme=calm)

*   Top languages

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra)

*   WakaTime card

![Harlok's wakatime stats](https://github-readme-stats.vercel.app/api/wakatime?username=ffflabs)

***
