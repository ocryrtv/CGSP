# CGSP Code Repository

This is code for CGSP(Cross-Domain Recommendation framework based on Graph Signal Processing).


## How to Run
To run the code, you can execute the following command in your terminal:

```bash
python main.py --dataset=<dataset name> --dtype=<src/tgt domain> --simple_model=<model name> --a=<alpha>
python main.py --dataset=amazon --dtype=movie_music --simple_model=cgsp-io --a=0.85
python main.py --dataset=douban --dtype=movie_book --simple_model=cgsp-oa --a=0.85
python main.py --dataset=amazon --dtype=sport_cloth --simple_model=cgsp-ua --a=0.85
