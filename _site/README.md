# minimal-days-theme

A minimalistic static [Jekyll](http://jekyllrb.com) blog theme! Displays full posts in single-column list.

Includes:
* pagination
* tags

![Preview](/minimal-theme-screenshot.png)

## Installation

Add this line to your Jekyll site's `Gemfile`:

```ruby
gem "minimal-days-theme"
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
theme: minimal-days-theme
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install minimal-days-theme

## Usage
### _config.yml options
General settings:
```
title: here & there                         # update title
title_img: assets/images/theme/cloud.gif    # update header image
```

Pagination:
```
paginate: 3                                 # change posts per page
```

### Images in posts
To insert a responsive image in a post:
```
{% responsive_image path:"assets/image/image.png" alt:"nice image bro" %}
```
When Jekyll builds the site, [jekyll-responsive-image](https://github.com/wildlyinaccurate/jekyll-responsive-image) will resize your images and load / display them in a responsive manner.

To insert an image / gif that should NOT be resized:
```
{% include image.html img="image.gif" description="check this out" %}
```

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

