# Musician

A Hugo Theme for Musicians

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
- [ ] media queries in contacts
- [ ] media queries in concerts
- [ ] media queries in photos
- [ ] media queries in videos
- [ ] BUG: language switch should stay on page
- [ ] year grouping on past concerts/list
- [ ] cookie policy
- [ ] footer band (see Toha)
- [ ] [Instagram User Token Generator](https://developers.facebook.com/docs/instagram-basic-display-api/overview#user-token-generator)
- [ ] share => ical
- [ ] replace Font Awesome with https://evil-icons.io/
- [ ] explore https://icomoon.io/

## Setup

```Powershell
cd C:\src\github.com\rebyv\site\
$hugoVersion = '0.100.1'
Set-Alias hugo "C:\bin\hugo\${hugoVersion}\hugo.exe"
#$env:PATH += ";C:\bin\sass_embedded;"
hugo serve
```

## Dependencies

- [flag-icons](https://github.com/lipis/flag-icons)  
- [Font Awesome 6.1.1 For The Web](https://fontawesome.com/)  
- ~~https://github.com/sass/dart-sass-embedded/releases~~
- https://getform.io/

# Ideas

[Hugo In Action](https://github.com/hugoinaction/hugoinaction)  
<http://template-method.webflow.io/>  
<https://hugocodex.org/>  
<https://css-tricks.com/>  
[Create A Dark/Light Mode Switch with CSS Variables](https://dev.to/ananyaneogi/create-a-dark-light-mode-switch-with-css-variables-34l8)  
<https://codepen.io/>  

## Instagram

Sharing a post Instagram is non-trivial.
see https://stackoverflow.com/a/66296656
and https://developers.facebook.com/docs/instagram-api/guides/content-publishing/


## Form services

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

## Structuring your Sass Projects

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

## Quick links

[Hugo bin](https://github.com/gohugoio/hugo/releases)  
[Hugo docs](https://gohugo.io/documentation/)  

[MDN](https://developer.mozilla.org/en-US/docs/Web/CSS)  
[SaSS](https://sass-lang.com/documentation/)  

### Calendar
<https://datatracker.ietf.org/doc/html/rfc5545>  
<https://datatracker.ietf.org/doc/html/rfc7986>  
<https://developer.mapquest.com/documentation/geocoding-api/address/get>  

### Fonts
<https://fonts.google.com/>  
<https://developers.google.com/fonts/docs/getting_started>  
<https://fontawesome.com/>  

### Misc
<https://tachyons-bootstrap.dwyl.com/>
<https://docs.netlify.com/>
<https://github.com/SVG-Edit/svgedit>

