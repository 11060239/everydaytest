Test Page for Everyday Listening
================

I am a big heading
==================

I am a smaller heading
----------------------

### I am even smaller

I am normal text

I am *italic* text. I am **bold** text.

-   I am a list item.
-   I am another list item.

``` r
library(tidyverse)
```

    ## Warning: package 'tidyverse' was built under R version 3.5.2

    ## ── Attaching packages ────────────────────────────────────────────────────────────────────────── tidyverse 1.3.0 ──

    ## ✓ ggplot2 3.2.1     ✓ purrr   0.3.3
    ## ✓ tibble  2.1.3     ✓ dplyr   0.8.4
    ## ✓ tidyr   1.0.2     ✓ stringr 1.4.0
    ## ✓ readr   1.3.1     ✓ forcats 0.4.0

    ## Warning: package 'ggplot2' was built under R version 3.5.2

    ## Warning: package 'tibble' was built under R version 3.5.2

    ## Warning: package 'tidyr' was built under R version 3.5.2

    ## Warning: package 'purrr' was built under R version 3.5.2

    ## Warning: package 'dplyr' was built under R version 3.5.2

    ## Warning: package 'stringr' was built under R version 3.5.2

    ## Warning: package 'forcats' was built under R version 3.5.2

    ## ── Conflicts ───────────────────────────────────────────────────────────────────────────── tidyverse_conflicts() ──
    ## x dplyr::filter() masks stats::filter()
    ## x dplyr::lag()    masks stats::lag()

``` r
library(spotifyr)
```

    ## Warning: package 'spotifyr' was built under R version 3.5.2

``` r
source('spotify.R')
```

``` r
#karaoke playlist: 3sJGjIN1wa9KszybCcj0hB
#chill playlist: 0TIMetHqr6J6S6QR19x8yi
chill_playlist = get_playlist_audio_features('11143302739','0TIMetHqr6J6S6QR19x8yi') 
karaoke_playlist = get_playlist_audio_features('11143302739','3sJGjIN1wa9KszybCcj0hB') 
chill_playlist
```

    ## # A tibble: 64 x 61
    ##    playlist_id playlist_name playlist_img playlist_owner_… playlist_owner_…
    ##    <chr>       <chr>         <chr>        <chr>            <chr>           
    ##  1 0TIMetHqr6… Chill         https://mos… 11143302739      11143302739     
    ##  2 0TIMetHqr6… Chill         https://mos… 11143302739      11143302739     
    ##  3 0TIMetHqr6… Chill         https://mos… 11143302739      11143302739     
    ##  4 0TIMetHqr6… Chill         https://mos… 11143302739      11143302739     
    ##  5 0TIMetHqr6… Chill         https://mos… 11143302739      11143302739     
    ##  6 0TIMetHqr6… Chill         https://mos… 11143302739      11143302739     
    ##  7 0TIMetHqr6… Chill         https://mos… 11143302739      11143302739     
    ##  8 0TIMetHqr6… Chill         https://mos… 11143302739      11143302739     
    ##  9 0TIMetHqr6… Chill         https://mos… 11143302739      11143302739     
    ## 10 0TIMetHqr6… Chill         https://mos… 11143302739      11143302739     
    ## # … with 54 more rows, and 56 more variables: danceability <dbl>,
    ## #   energy <dbl>, key <int>, loudness <dbl>, mode <int>,
    ## #   speechiness <dbl>, acousticness <dbl>, instrumentalness <dbl>,
    ## #   liveness <dbl>, valence <dbl>, tempo <dbl>, track.id <chr>,
    ## #   analysis_url <chr>, time_signature <int>, added_at <chr>,
    ## #   is_local <lgl>, primary_color <lgl>, added_by.href <chr>,
    ## #   added_by.id <chr>, added_by.type <chr>, added_by.uri <chr>,
    ## #   added_by.external_urls.spotify <chr>, track.artists <list>,
    ## #   track.available_markets <list>, track.disc_number <int>,
    ## #   track.duration_ms <int>, track.episode <lgl>, track.explicit <lgl>,
    ## #   track.href <chr>, track.is_local <lgl>, track.name <chr>,
    ## #   track.popularity <int>, track.preview_url <chr>, track.track <lgl>,
    ## #   track.track_number <int>, track.type <chr>, track.uri <chr>,
    ## #   track.album.album_type <chr>, track.album.artists <list>,
    ## #   track.album.available_markets <list>, track.album.href <chr>,
    ## #   track.album.id <chr>, track.album.images <list>,
    ## #   track.album.name <chr>, track.album.release_date <chr>,
    ## #   track.album.release_date_precision <chr>,
    ## #   track.album.total_tracks <int>, track.album.type <chr>,
    ## #   track.album.uri <chr>, track.album.external_urls.spotify <chr>,
    ## #   track.external_ids.isrc <chr>, track.external_urls.spotify <chr>,
    ## #   video_thumbnail.url <lgl>, key_name <chr>, mode_name <chr>,
    ## #   key_mode <chr>

``` r
karaoke_playlist
```

    ## # A tibble: 110 x 61
    ##    playlist_id playlist_name playlist_img playlist_owner_… playlist_owner_…
    ##    <chr>       <chr>         <chr>        <chr>            <chr>           
    ##  1 3sJGjIN1wa… Karaoke       https://mos… 11143302739      11143302739     
    ##  2 3sJGjIN1wa… Karaoke       https://mos… 11143302739      11143302739     
    ##  3 3sJGjIN1wa… Karaoke       https://mos… 11143302739      11143302739     
    ##  4 3sJGjIN1wa… Karaoke       https://mos… 11143302739      11143302739     
    ##  5 3sJGjIN1wa… Karaoke       https://mos… 11143302739      11143302739     
    ##  6 3sJGjIN1wa… Karaoke       https://mos… 11143302739      11143302739     
    ##  7 3sJGjIN1wa… Karaoke       https://mos… 11143302739      11143302739     
    ##  8 3sJGjIN1wa… Karaoke       https://mos… 11143302739      11143302739     
    ##  9 3sJGjIN1wa… Karaoke       https://mos… 11143302739      11143302739     
    ## 10 3sJGjIN1wa… Karaoke       https://mos… 11143302739      11143302739     
    ## # … with 100 more rows, and 56 more variables: danceability <dbl>,
    ## #   energy <dbl>, key <int>, loudness <dbl>, mode <int>,
    ## #   speechiness <dbl>, acousticness <dbl>, instrumentalness <dbl>,
    ## #   liveness <dbl>, valence <dbl>, tempo <dbl>, track.id <chr>,
    ## #   analysis_url <chr>, time_signature <int>, added_at <chr>,
    ## #   is_local <lgl>, primary_color <lgl>, added_by.href <chr>,
    ## #   added_by.id <chr>, added_by.type <chr>, added_by.uri <chr>,
    ## #   added_by.external_urls.spotify <chr>, track.artists <list>,
    ## #   track.available_markets <list>, track.disc_number <int>,
    ## #   track.duration_ms <int>, track.episode <lgl>, track.explicit <lgl>,
    ## #   track.href <chr>, track.is_local <lgl>, track.name <chr>,
    ## #   track.popularity <int>, track.preview_url <chr>, track.track <lgl>,
    ## #   track.track_number <int>, track.type <chr>, track.uri <chr>,
    ## #   track.album.album_type <chr>, track.album.artists <list>,
    ## #   track.album.available_markets <list>, track.album.href <chr>,
    ## #   track.album.id <chr>, track.album.images <list>,
    ## #   track.album.name <chr>, track.album.release_date <chr>,
    ## #   track.album.release_date_precision <chr>,
    ## #   track.album.total_tracks <int>, track.album.type <chr>,
    ## #   track.album.uri <chr>, track.album.external_urls.spotify <chr>,
    ## #   track.external_ids.isrc <chr>, track.external_urls.spotify <chr>,
    ## #   video_thumbnail.url <lgl>, key_name <chr>, mode_name <chr>,
    ## #   key_mode <chr>
