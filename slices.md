# Slice Guidelines

## Naming

Slices should be named to be as meaningful as possible for users. Imagine a user clicking
the "Add a slice" selector — the name that appears there should describe exactly what sort
of content the slice will add to the page.

We have some preferred names for common slices:

* `TextSlice`
* `ImagesSlice`
* `TitleSlice`
* `DividerSlice`

## Markup

Slices should be wrapped in a div container with the appropriate class.

```html
<div class="text">
  ...
</div>

<div class="post-set">
  ...
</div>
```

Note we’re using hyphenated class names, rather than underscored.

## Stylesheets

The styles for a slice go in `app/assets/stylesheets/slices/slice_name.scss`.
This should mirror the path in `app/slices`.
For example: `app/assets/stylesheets/slices/text.scss`.
These styles will be concatenated into `application.css`.

## Javascripts

Javascripts follow the same rule as stylesheets. If a slice has no extra
javascript behaviour, do not create a placeholder file.
