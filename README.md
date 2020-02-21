Test Page for Everyday Listening
================

My playlists
------------

Of all my playlists on Spotify, there are two that I like to listen to the most. One is called *Chill* and the other is called *Karaoke*. *Chill* contains a lot of songs to relax to. I think these are slower, acoustic songs, possibly played in minor more often than major. I think the songs in *Karaoke* are more energetic, maybe easier to dance to and also louder. Let's see if the Spotify API would say the same.

``` r
spotify_features %>% 
  ## Try grouping by group member and/or year.
  group_by(type) %>% 
  ## Try different features and different summary functions.
  summarise(Tempo=mean(tempo), Acousticness=mean(acousticness), Mode=mean(mode), Energy=mean(energy), Danceability=mean(danceability), Loudness=mean(loudness))
```

    ## # A tibble: 2 x 7
    ##   type    Tempo Acousticness  Mode Energy Danceability Loudness
    ##   <chr>   <dbl>        <dbl> <dbl>  <dbl>        <dbl>    <dbl>
    ## 1 Chill    110.        0.606 0.688  0.370        0.624   -11.2 
    ## 2 Karaoke  121.        0.175 0.664  0.722        0.618    -6.45
