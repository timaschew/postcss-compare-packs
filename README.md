# postcss-compare-packs

Compare most popular [PostCSS][1] packs like cssnext, rucksack and precss

| PostCSS Plugin             | [postcss-cssnext][2]           | [rucksack][3]                  | [precss][4]          |
| -------------------------- | ------------------------------ | ------------------------------ | -------------------- |
| [autoprefixer][10]           | :white_check_mark:             | :white_check_mark:             |                      |
| [laggard][11]                |                                | :white_check_mark:             |                      |
| [pixrem][12]                 | :white_check_mark:             |                                |                      |
| [pleeease-filters][13]       | :white_check_mark:             |                                |                      |
| [-advanced-variables][14]    |                                |                                |  :white_check_mark:  |
| [-alias][15]                 |                                | :white_check_mark:             |                      |
| [-atroot][16]                |                                |                                |  :white_check_mark:  |
| [-calc][17]                  | :white_check_mark:             |                                |                      |
| [-clearfix][18]              |                                | :white_check_mark:             |                      |
| [-color-function][19]        | :white_check_mark:             |                                | :white_check_mark:   |
| [-color-gray][20]            | :white_check_mark:             |                                |                      |
| [-color-hex-alpha][21]       | :white_check_mark:             |                                |                      |
| [-color-hwb][22]             | :white_check_mark:             |                                |                      |
| [-color-rebeccapurple][23]   | :white_check_mark:             |                                |                      |
| [-color-rgba-fallback][24]   | :white_check_mark:             |                                |                      |
| [-custom-media][25]          | :white_check_mark:             |                                | :white_check_mark:   |
| [-custom-properties][26]     | :white_check_mark:             |                                | :white_check_mark:   |
| [-custom-selectors][27]      | :white_check_mark:             |                                | :white_check_mark:   |
| [-easings][28]               |                                | :white_check_mark:             |                      |
| [-extend][29]                |                                |                                |  :white_check_mark:  |
| [-font-variant][30]          | :white_check_mark:             |                                |                      |
| [-fontpath][31]              |                                | :white_check_mark:             |                      |
| [-hexrgba][32]               |                                | :white_check_mark:             |                      |
| [-initial][33]               | :white_check_mark:             |                                |                      |
| [-input-style][34]           |                                | :white_check_mark:             |                      |
| [-media-minmax][35]          | :white_check_mark:             |                                |  :white_check_mark:  |
| [-mixins][36]                |                                |                                |  :white_check_mark:  |
| [-nested][37]                |                                |                                |  :white_check_mark:  |
| [-nesting][38]               | :white_check_mark:             |                                |  :white_check_mark:  |
| [-partial-import][39]        |                                |                                |  :white_check_mark:  |
| [-position][40]              |                                | :white_check_mark:             |                      |
| [-property-lookup][41]       |                                | :white_check_mark:             |                      |
| [-pseudo-class-any-link][42] | :white_check_mark:             |                                |                      |
| [-pseudoelements][43]        | :white_check_mark:             |                                |                      |
| [-quantity-queries][44]      |                                | :white_check_mark:             |                      |
| [-responsive-type][45]       |                                | :white_check_mark:             |                      |
| [-selector-matches][46]      | :white_check_mark:             |                                |  :white_check_mark:  |
| [-selector-not][47]          | :white_check_mark:             |                                |  :white_check_mark:  |


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


[1]: http://postcss.org/
[2]: http://cssnext.io/
[3]: http://simplaio.github.io/rucksack/
[4]: https://jonathantneal.github.io/precss/
[10]: https://www.npmjs.com/package/autoprefixer           
[11]: https://www.npmjs.com/package/laggard                
[12]: https://www.npmjs.com/package/pixrem                 
[13]: https://www.npmjs.com/package/pleeease-filters       
[14]: https://www.npmjs.com/package/postcss-advanced-variables  
[15]: https://www.npmjs.com/package/postcss-alias                 
[16]: https://www.npmjs.com/package/postcss-atroot                
[17]: https://www.npmjs.com/package/postcss-calc                  
[18]: https://www.npmjs.com/package/postcss-clearfix              
[19]: https://www.npmjs.com/package/postcss-color-function        
[20]: https://www.npmjs.com/package/postcss-color-gray            
[21]: https://www.npmjs.com/package/postcss-color-hex-alpha       
[22]: https://www.npmjs.com/package/postcss-color-hwb             
[23]: https://www.npmjs.com/package/postcss-color-rebeccapurple   
[24]: https://www.npmjs.com/package/postcss-color-rgba-fallback   
[25]: https://www.npmjs.com/package/postcss-custom-media          
[26]: https://www.npmjs.com/package/postcss-custom-properties     
[27]: https://www.npmjs.com/package/postcss-custom-selectors      
[28]: https://www.npmjs.com/package/postcss-easings               
[29]: https://www.npmjs.com/package/postcss-extend                
[30]: https://www.npmjs.com/package/postcss-font-variant          
[31]: https://www.npmjs.com/package/postcss-fontpath              
[32]: https://www.npmjs.com/package/postcss-hexrgba               
[33]: https://www.npmjs.com/package/postcss-initial               
[34]: https://www.npmjs.com/package/postcss-input-style           
[35]: https://www.npmjs.com/package/postcss-media-minmax          
[36]: https://www.npmjs.com/package/postcss-mixins                
[37]: https://www.npmjs.com/package/postcss-nested                
[38]: https://www.npmjs.com/package/postcss-nesting               
[39]: https://www.npmjs.com/package/postcss-partial-import        
[40]: https://www.npmjs.com/package/postcss-position              
[41]: https://www.npmjs.com/package/postcss-property-lookup       
[42]: https://www.npmjs.com/package/postcss-pseudo-class-any-link 
[43]: https://www.npmjs.com/package/postcss-pseudoelements        
[44]: https://www.npmjs.com/package/postcss-quantity-queries      
[45]: https://www.npmjs.com/package/postcss-responsive-type       
[46]: https://www.npmjs.com/package/postcss-selector-matches      
[47]: https://www.npmjs.com/package/postcss-selector-not   
