# CGSP Code Repository

This is code for CGSP(Cross-Domain Recommendation framework based on Graph Signal Processing).
Also this code includes 3 basedlines of GSP-based methods(i.e, GF-CF, PGSP, LGCN-IDE) for unified domain.


## Datasets
We have used two datasets : [Amazon](http://jmcauley.ucsd.edu/data/amazon/index_2014.html) and [Douban](https://www.kaggle.com/datasets/fengzhujoey/douban-datasetratingreviewside-information?resource=download)
You can put data in `cgsp/data/` with `{dataset}_{source domain}_{target domain}_{train/val/test}_{test_mode}.csv` format.

## How to Run
To run the code, you can execute the following command in your terminal:-
- test_mode : `src` for inter-domain recommendation, `tgt` for intra-domain recommendation
- simple_model : cgsp-io, cgsp-oa, cgsp-ua
- Additionally, if you want to test previous GSP-methods in unified domain, you can execute command with `--simple_model={gf-cf/pgsp/lgcn-ide} --test_mode={merge-src/merge-tgt}`

```bash
python main.py --dataset=<dataset name> --dtype=<src/tgt domain> --simple_model=<model name> --a=<alpha> --test_mode=<src/tgt>
python main.py --dataset=amazon --dtype=movie_music --simple_model=cgsp-io --a=0.85
python main.py --dataset=douban --dtype=movie_book --simple_model=cgsp-oa --a=0.85
python main.py --dataset=amazon --dtype=sport_cloth --simple_model=cgsp-ua --a=0.85
