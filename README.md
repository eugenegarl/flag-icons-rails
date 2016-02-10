FlagIconsRails
---

This project integrates [https://github.com/lipis/flag-icon-css](https://github.com/lipis/flag-icon-css) in a Ruby Gem but only the sass version.

**THIS GEM IS IN EARLY BETA STATE SO USE AT YOUR OWN RISK**

### Installation

In your Gemfile include:

```ruby
gem 'flag-icons-rails'
```

And then execute:

```sh
bundle install
```

Import the FlagIconsRails styles in your `app/assets/stylesheets/application.scss`.

```scss
@import "flag-icons-rails";
```

#### Plain usage

In your view:

```html
<span class="flag-icon flag-icon-it"></span>
```

```html
<span class="flag-icon flag-icon-it flag-icon-squared"></span>
```

#### Rails Helper usage

In your view:

```ruby
flag_icon(:it)
# => <span class="flag-icon flag-icon-it"></span>
```

```ruby
flag_icon(:it, true)
# => <span class="flag-icon flag-icon-it flag-icon-squared"></span>
```

```ruby
flag_icon(:it, id: 'my-flag', class: 'strong')
# => <span id="my-flag" class="flag-icon flag-icon-it flag-icon-squared strong"></span>
```

### Thanks

* [lipis/flag-icon-css](https://github.com/lipis/flag-icon-css) for flags-icon-css
* [flag-icon-sass gem](https://github.com/cfiorini/flag-icon-sass) for gem this one is based on
