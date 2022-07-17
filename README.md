# Musician

A Hugo Theme for Musicians


## Implementation Details

### Favicon

suggestion from https://evilmartians.com/chronicles/how-to-favicon-in-2021-six-files-that-fit-most-needs
basic favicon: 32×32
SVG except mobiles
Apple touch icon: 180×180
Android devices: 192×192 and 512×512

### Run-time Dependencies

- [flag-icons](https://github.com/lipis/flag-icons)  
- [Font Awesome 6.1.1 For The Web](https://fontawesome.com/)  
- https://getform.io/  

### Build-time Dependencies

- [Hugo]  
- [MapQuest API](https://developer.mapquest.com/)  


### Dev Setup

```Powershell
cd C:\src\github.com\rebyv\site\
$hugoVersion = '0.100.1'
Set-Alias hugo "C:\bin\hugo\${hugoVersion}\hugo.exe"
#$env:PATH += ";C:\bin\sass_embedded;"
hugo serve
```

#### Quick links

[Hugo bin](https://github.com/gohugoio/hugo/releases)  
[Hugo docs](https://gohugo.io/documentation/)  

[MDN](https://developer.mozilla.org/en-US/docs/Web/CSS)  
[SaSS](https://sass-lang.com/documentation/)  

#### Calendar (.ics)

- <https://datatracker.ietf.org/doc/html/rfc5545>  
- <https://datatracker.ietf.org/doc/html/rfc7986>  
- <https://developer.mapquest.com/documentation/geocoding-api/address/get>  

## Ideas for Improvements

[Hugo In Action](https://github.com/hugoinaction/hugoinaction)  
<http://template-method.webflow.io/>  
<https://hugocodex.org/>  
<https://css-tricks.com/>  
[Create A Dark/Light Mode Switch with CSS Variables](https://dev.to/ananyaneogi/create-a-dark-light-mode-switch-with-css-variables-34l8)  
<https://codepen.io/>  

### Add Instagram

Sharing a post Instagram is non-trivial.
see https://stackoverflow.com/a/66296656
and https://developers.facebook.com/docs/instagram-api/guides/content-publishing/
- [ ] [Instagram User Token Generator](https://developers.facebook.com/docs/instagram-basic-display-api/overview#user-token-generator)

### How to structure Sass Project

[Structuring your Sass Projects](https://itnext.io/structuring-your-sass-projects-c8d41fa55ed4)

```
sass/
|
|– abstracts/ (or utilities/)
|   |– _variables.scss    // Sass Variables
|   |– _functions.scss    // Sass Functions
|   |– _mixins.scss       // Sass Mixins
|
|– base/
|   |– _reset.scss        // Reset/normalize
|   |– _typography.scss   // Typography rules
|
|– components/ (or modules/)
|   |– _buttons.scss      // Buttons
|   |– _carousel.scss     // Carousel
|   |– _slider.scss       // Slider
|
|– layout/
|   |– _navigation.scss   // Navigation
|   |– _grid.scss         // Grid system
|   |– _header.scss       // Header
|   |– _footer.scss       // Footer
|   |– _sidebar.scss      // Sidebar
|   |– _forms.scss        // Forms
|
|– pages/
|   |– _home.scss         // Home specific styles
|   |– _about.scss        // About specific styles
|   |– _contact.scss      // Contact specific styles
|
|– themes/
|   |– _theme.scss        // Default theme
|   |– _admin.scss        // Admin theme
|
|– vendors/
|   |– _bootstrap.scss    // Bootstrap
|   |– _jquery-ui.scss    // jQuery UI
|
`– main.scss              // Main Sass file
```

```scss
@import 'abstracts/variables';
@import 'abstracts/functions';
@import 'abstracts/mixins';

@import 'vendors/bootstrap';
@import 'vendors/jquery-ui';

@import 'base/reset';
@import 'base/typography';

@import 'layout/navigation';
@import 'layout/grid';
@import 'layout/header';
@import 'layout/footer';
@import 'layout/sidebar';
@import 'layout/forms';

@import 'components/buttons';
@import 'components/carousel';
@import 'components/slider';

@import 'pages/home';
@import 'pages/about';
@import 'pages/contact';

@import 'themes/theme';
@import 'themes/admin';
```


### Fonts
<https://fonts.google.com/>  
<https://developers.google.com/fonts/docs/getting_started>  
<https://fontawesome.com/>  

### Misc
<https://tachyons-bootstrap.dwyl.com/>
<https://tailwind-elements.com/>
<https://docs.netlify.com/>
<https://github.com/SVG-Edit/svgedit>

### Icons

- <https://evil-icons.io/>
- <https://icomoon.io/>
- <https://developers.google.com/fonts/docs/material_symbols>
- <https://developers.google.com/fonts/docs/material_icons>

## Research

### Form services

- https://getform.io/ => plain HTML => only 50!
- https://formspree.io/ => plain HTML => ?
- https://formester.com/ => plain HTML => ?
- https://www.99inbound.com/ => plain HTML => ?
- https://kwesforms.com/ => include JS -> :-(
- https://formium.io/ => Javascript API -> :-(
- Netlify Forms => must publish in Netlify -> :-(
- Google Forms => plain HTML => reverse engineering -> :-(
- hugo-moodlebox-theme => DYI => need backend, e.g. zapier -> :-(
- zapier => form SaaS -> :-(
- zapier => webjooks => Premium -> :-(

## TODO

- [x] Share -LinkedIn +Instagram
- [x] social links
- [x] footer since
- [x] archetypes `hugo new content\concerts\2023-01-01\dublin.en.md -k concert`
- [x] favicon
- [x] style concert/single
- [x] pic&vid card-style
- [x] BUG: video card are bad
- [x] 404
  > photo-1558458878-36802fc5f7f5.jfif (@ Unsplash by Marina Reich)
- [x] background images scaling
- [x] contacts for mobile
- [x] BUG: language switch should stay on page
- [x] concerts layout for mobile
- [x] Staging
- [x] year grouping on past concerts/list
- [x] home section: concerts
- [ ] sticky footer on small device
- [x] home section: videos
- [x] home section: bio
- [x] sections: do not repeat background pic, section height fraction of viewport height
- [ ] cookie policy (=> youtube)
- [ ] reconsider icons
- [ ] https://www.toptal.com/developers/webdevchecklist
- [ ] replace CSS with https://bulma.io/
- [ ] footer band (see Toha)