# Image and PDF tricks on Linux

## Generic Commands

### List file in smart order

This sorts "im11" before "im100"

```sh
ls -v1
```

## Imagemagick

Use `convert` to save separaetly and `mogrify` to edit in place

### Split image into left and right halves

```sh
mogrify -crop 50%x100% +repage $(ls -v1)
```

### Change image resolution
