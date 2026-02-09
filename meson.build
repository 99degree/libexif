project('libexif', 'c',
  version : '0.6.24',
  license : 'LGPL'
)

# Include directory
inc = include_directories('libexif')

# Source files (from Android.bp)
srcs = files(
  'libexif/exif-data.c',
  'libexif/exif-entry.c',
  'libexif/exif-ifd.c',
  'libexif/exif-loader.c',
  'libexif/exif-log.c',
  'libexif/exif-mnote-data.c',
  'libexif/exif-mnote-data-priv.c',
  'libexif/exif-tag.c',
  'libexif/exif-utils.c',
  'libexif/exif-byte-order.c',
  'libexif/exif-content.c',
  'libexif/exif-format.c',
  'libexif/exif-mem.c',
  'libexif/exif-mnote-data-canon.c',
  'libexif/exif-mnote-data-olympus.c',
  'libexif/exif-mnote-data-pentax.c',
  'libexif/exif-mnote-data-nikon.c',
  'libexif/exif-mnote-data-nikon2.c',
  'libexif/exif-mnote-data-fuji.c',
  'libexif/exif-mnote-data-sanyo.c',
  'libexif/exif-mnote-data-casio.c',
  'libexif/exif-mnote-data-minolta.c',
  'libexif/exif-mnote-data-panasonic.c',
  'libexif/exif-mnote-data-sigma.c',
  'libexif/exif-mnote-data-sony.c',
  'libexif/exif-mnote-data-kodak.c',
  'libexif/exif-mnote-data-leica.c'
)

# Build the library
libexif = library(
  'exif',
  srcs,
  include_directories : inc,
  install : true,
)

# Provide dependency object
libexif_dep = declare_dependency(
  link_with : libexif,
  include_directories : inc,
)

# Install headers (from Android.bp)
install_headers(
  files(
    'libexif/exif-data.h',
    'libexif/exif-entry.h',
    'libexif/exif-ifd.h',
    'libexif/exif-loader.h',
    'libexif/exif-log.h',
    'libexif/exif-mnote-data.h',
    'libexif/exif-tag.h',
    'libexif/exif-utils.h',
    'libexif/exif-byte-order.h',
    'libexif/exif-content.h',
    'libexif/exif-format.h',
    'libexif/exif-mem.h'
  ),
  subdir : 'libexif'
)
