# 8-point
A set of 8 point grid classes.

## Why

[8-point grid](https://spec.fm/specifics/8-pt-grid) is a thing.
It's a good thing at that.

8 has a lot of advantages as a number.
It's chief adavntage is that it bifurcates evenly.
So devices that do any type of strange scaling don't end up with half-values.

This is good.

This lib just offers a set of classes for using an 8-point soft grid with the css box model. It incluedes classes for `margin`, `padding`, `TRBL`, `width`, `height`, and "size".

## Anatomy

The class names break down like this:

```txt
{acronymized CSS property}-{n × .5rem}
```

For example:

```css
.p-1 { padding:  .5rem }  /* 1 × .5rem */
.p-2 { padding: 1rem } /* 2 × .5rem */
.p-3 { padding: 1.5rem } /* 3 × .5rem */
```

You can use side-specific properties as well:

```css
.mt-1 { margin-top: .5rem }
.mr-1 { margin-right: .5rem }
.mb-1 { margin-bottom: .5rem }
.ml-1 { margin-left: .5rem }

/* x and y added for convenience */

.my-1 { margin-top: .5rem; margin-bottom: .5rem }
.mx-1 { margin-right: .5rem; margin-left: .5rem }
```

## Legend

#### properties

```txt
m  = margin
mt = margin-top
mr = margin-right
mb = margin-bottom
ml = margin-left
my = margin-top; margin-bottom
mx = margin-right; margin-left

p  = padding
pt = padding-top
pr = padding-right
pb = padding-bottom
pl = padding-left
py = padding-top; padding-bottom
px = padding-right; margin-left

t = top
r = right
b = bottom
l = left

w = width
h = height

s = width; height
```

#### values

```txt
1 = .5rem
2 = 1rem
3 = 1.5rem
4 = 2rem
5 = 2.5rem
6 = 3rem
7 = 3.5rem
8 = 4rem
```

## Install
NPM:
`npm i -S 8-point`

## Use
```html
<div class="m-1 p-3">
  This has .5rem margin and 1.5rem padding.
</div>

<img
  src="./path/img.ext"
  class="s-8"
  alt="this img is 4rem high and wide"
/>
```

## License

MIT License

Copyright (c) 2016 Michael Chan
