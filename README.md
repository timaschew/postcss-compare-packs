# postcss-compare-packs

Compare most popular [PostCSS][1] packs like cssnext, rucksack and precss

| PostCSS Plugin         | [postcss-cssnext][2]           | [rucksack][3]                  | [precss][4]          |
| ---------------------- | ------------------------------ | ------------------------------ | -------------------- |
| autoprefixer           | :white_check_mark:             | :white_check_mark:             |                      |
| laggard                |                                | :white_check_mark:             |                      |
| pixrem                 | :white_check_mark:             |                                |                      |
| pleeease-filters       | :white_check_mark:             |                                |                      |
| -advanced-variables    |                                |                                |  :white_check_mark:  |
| -alias                 |                                | :white_check_mark:             |                      |
| -atroot                |                                |                                |  :white_check_mark:  |
| -calc                  | :white_check_mark:             |                                |                      |
| -clearfix              |                                | :white_check_mark:             |                      |
| -color-function        | :white_check_mark:             |                                | :white_check_mark:   |
| -color-gray            | :white_check_mark:             |                                |                      |
| -color-hex-alpha       | :white_check_mark:             |                                |                      |
| -color-hwb             | :white_check_mark:             |                                |                      |
| -color-rebeccapurple   | :white_check_mark:             |                                |                      |
| -color-rgba-fallback   | :white_check_mark:             |                                |                      |
| -custom-media          | :white_check_mark:             |                                | :white_check_mark:   |
| -custom-properties     | :white_check_mark:             |                                | :white_check_mark:   |
| -custom-selectors      | :white_check_mark:             |                                | :white_check_mark:   |
| -easings               |                                | :white_check_mark:             |                      |
| -extend                |                                |                                |  :white_check_mark:  |
| -font-variant          | :white_check_mark:             |                                |                      |
| -fontpath              |                                | :white_check_mark:             |                      |
| -hexrgba               |                                | :white_check_mark:             |                      |
| -initial               | :white_check_mark:             |                                |                      |
| -input-style           |                                | :white_check_mark:             |                      |
| -media-minmax          | :white_check_mark:             |                                |  :white_check_mark:  |
| -mixins                |                                |                                |  :white_check_mark:  |
| -nested                |                                |                                |  :white_check_mark:  |
| -nesting               | :white_check_mark:             |                                |  :white_check_mark:  |
| -partial-import        |                                |                                |  :white_check_mark:  |
| -position              |                                | :white_check_mark:             |                      |
| -property-lookup       |                                | :white_check_mark:             |                      |
| -pseudo-class-any-link | :white_check_mark:             |                                |                      |
| -pseudoelements        | :white_check_mark:             |                                |                      |
| -quantity-queries      |                                | :white_check_mark:             |                      |
| -responsive-type       |                                | :white_check_mark:             |                      |
| -selector-matches      | :white_check_mark:             |                                |  :white_check_mark:  |
| -selector-not          | :white_check_mark:             |                                |  :white_check_mark:  |


##### What does it mean if a plugin exists in more than one pack?

Assuming that each pack should focus on just one topic, it's an indicator that
this strategy was not achieved or the topic was chosen in a wrong aspect. Read more in the [PostCSS Plugin Guideline - Do one thing, and do it well](https://github.com/postcss/postcss/blob/master/docs/guidelines/plugin.md#12-do-one-thing-and-do-it-well)

##### Can I use multiple packs at once?

Yes.
You might need to figure out in which order you need to use them.

##### If I use multiple packs does the order matter?
It depends on the plugin(s). Some plugins contains a note in the Readme like [postcss-import](https://github.com/postcss/postcss-import). 
If you want to use _precss_ and _cssnext_, _precss_ need to be loaded __before__ _cssnext_.

##### What does happen to the output if a plugin is executed by more than one pack?

It depends on the plugin. But the autoprefixer for instance 
doesn't do anything if it will process the data a second time.

##### Can I disable particular plugins within a pack?

Every pack should provide an options argument to disable particular plugnis.


##### TODO

- add links to plugins 
- add links to packs

[1]: https://github.com/postcss/postcss
