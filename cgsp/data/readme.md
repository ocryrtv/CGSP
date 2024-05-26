
The given dataset is randomly sampled version of `Amazon Movie`(source domain) and `Amazon Music`(target domain).

You can put data in cgsp/data/ with {dataset}_{source domain}_{target domain}_{train/val/test}_{test_mode}.csv format.
- dataset : Douban or Amazon
- source domain : movie/sports 
- target domain : music/book/clothes
- test_mode : 'src' for inter-domain recommendaation, 'tgt' for intra-domain recommendation
