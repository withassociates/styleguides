# Slice Guidelines

## Naming

Slice names should be singular if possible.
i.e. `TextSlice` and `ImageSlice`.

This goes for set slices too. So for a blog we’d create a
`PostSetSlice`, for event listings `EventSetSlice`.

We have some preferred names for common slices:

* `TextSlice`
* `ImageSlice`
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
